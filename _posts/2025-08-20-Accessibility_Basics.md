---
layout: post
title: "Accessibility Basics Every App Developer Should Know (in .NET MAUI)"
categories: [Article, Accessibility]
image: assets/images/Accessibility.png
---


Accessibility often gets treated like documentation: everyone agrees
it's important, but it's the first thing to slip off the sprint board
when deadlines loom. The truth is, if you're building apps in .NET MAUI,
accessibility isn't just about compliance - it's about making sure your
users can actually *use* your app. After all, a feature nobody can
access isn't really a feature.

For context: these articles are me working through my own project (a
project management app), documenting what I learn along the way. This
one is a list of accessibility implementations every .NET developer
should know - and, ideally, should ship.

------------------------------------------------------------------------

## Labels That Actually Say Something

Accessibility starts with labels. If your button just says "Click me,"
congratulations, you've built an Easter egg hunt for screen reader
users. Every actionable element should describe what it *does*. For
example, if you have a button to start a sprint, make it "Start Sprint,"
not "Go." Your future self (and your users) will thank you.

``` xml
<Button Text="Start Sprint" 
        SemanticProperties.Hint="Starts the current sprint for your project"/>
```

The `Hint` gives users extra context, so when a screen reader announces
it, they know exactly what's about to happen.

------------------------------------------------------------------------

## Button Size: Bigger Really Is Better

Tiny tap targets are the enemy of accessibility (and thumbs in general).
Apple recommends a minimum of 44x44 points, and Google suggests 48x48
dp. If your "Complete Task" button is smaller than a Tic Tac, it's time
for a redesign.

``` xml
<Button Text="Complete Task"
        HeightRequest="48"
        WidthRequest="120"/>
```

You're not designing for ants. Make your buttons large enough to hit on
the first try, even if the user's on a crowded train with one hand on
their coffee.

------------------------------------------------------------------------

## Color Contrast Isn't Optional

That pastel grey text on a white background might look "modern" in your
Figma mockup, but for someone with low vision, it's basically invisible.
WCAG guidelines recommend a contrast ratio of at least 4.5:1 for normal
text.

Pro tip: test your color combos with tools like [Contrast
Checker](https://webaim.org/resources/contrastchecker/) or the
[Accessibility Insights extension](https://accessibilityinsights.io/).
If your "Start Sprint" text looks like a ghost whisper, crank up the
contrast.

------------------------------------------------------------------------

## Don't Rely on Swipe Gestures Alone

Swipe gestures are slick, but not everyone can (or wants to) use them.
If "swipe left to complete a task" is your only option, you're locking
out users. Always provide an alternative action, like a button.

``` xml
<SwipeView>
    <SwipeView.RightItems>
        <SwipeItems>
            <SwipeItem Text="Complete"
                       IconImageSource="check.png"
                       Command="{Binding CompleteTaskCommand}" />
        </SwipeItems>
    </SwipeView.RightItems>
</SwipeView>

<Button Text="Complete Task"
        Command="{Binding CompleteTaskCommand}" />
```

Now both power users and accessibility users are covered. Everybody
wins.

------------------------------------------------------------------------

## Test With a Screen Reader (Seriously)

This isn't optional. Turn on VoiceOver (iOS) or TalkBack (Android) and
actually use your app. You'll quickly learn whether your "Add Sprint"
button announces itself clearly or just reads out "Button 17 of 42."
Spoiler: the latter isn't helpful.

------------------------------------------------------------------------

## Keep Your Layouts Simple

Complex nested layouts can confuse assistive tech. Stick to clean,
logical structures. For example, group related controls (like sprint
details) in a container with a semantic description.

``` xml
<VerticalStackLayout SemanticProperties.Description="Sprint details section">
    <Label Text="Sprint Name" />
    <Label Text="Ends in 5 days" />
</VerticalStackLayout>
```

This helps users understand the context without needing to explore every
label individually.

------------------------------------------------------------------------

## Pro Tip: Community Toolkit

The [.NET MAUI Community
Toolkit](https://learn.microsoft.com/dotnet/communitytoolkit/maui/) has
some excellent helpers for accessibility and beyond. Before reinventing
the wheel (badly), check if someone's already solved your problem.

------------------------------------------------------------------------

## References & Further Reading

-   [WCAG Guidelines](https://www.w3.org/WAI/standards-guidelines/wcag/)
-   [Microsoft Docs on Accessibility in .NET
    MAUI](https://learn.microsoft.com/dotnet/maui/fundamentals/accessibility)
-   [Accessibility Insights](https://accessibilityinsights.io/)
-   [WebAIM Contrast
    Checker](https://webaim.org/resources/contrastchecker/)

------------------------------------------------------------------------

## Final Thoughts

Accessibility isn't a "nice-to-have" it's table stakes. If your
project management app can start sprints, complete tasks, and keep
deadlines, it should also let *everyone* actually interact with it.
Think of it like this: you wouldn't build a project board where only
some team members can move tickets. Don't build an app where only some
users can take part.

Do the work now, save yourself the awkward support emails later.
