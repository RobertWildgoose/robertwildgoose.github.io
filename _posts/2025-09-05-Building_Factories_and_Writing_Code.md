---
layout: post
title: "Building Factories and Writing Code: How Satisfactory Aligns with SOLID Principles"
categories: [Article, Programming]
image: assets/images/Building_Factories.png
---


Ever spent hours optimising a conveyor belt in *Satisfactory*… only to realise it feels a lot like debugging code?

A coworker said last week that he doesn’t like the game because it feels too much like work. That got me thinking: why does building factories in a game mirror so many aspects of coding?

This game starts on a fresh alien planet, brand new to you, similar to landing your first role. You think you’re prepared from your studies, but suddenly you’re in the wild with new creatures, resources, and challenges. It turns out *Satisfactory* aligns surprisingly well with the **SOLID principles** and software development best practices.

---

### **1. Start Small, Iterate Often (Single Responsibility Principle)**

In *Satisfactory*, you begin with nothing but a handheld tool and your own two hands to gather leaves. A clean slate, but still just the beginning.

From there, you expand your factory step by step, adding machines and conveyor belts, refining layouts as you learn. Each section has a focused purpose.

That’s the **Single Responsibility Principle** in action: start simple, let each component do one thing well, and iterate as you grow.

---

### **2. Build Modules, Not Monoliths (Open/Closed Principle)**

As your factory grows, it naturally splits into modules, smelting areas, constructor lines, assembly zones. Each one has a clear role, and you can extend them by adding another machine or conveyor without tearing the whole thing down.

That’s the **Open/Closed Principle**: systems should be **open for extension but closed for modification**. You don’t rewrite the old smelting line, you add a new one, or scale horizontally. This modular approach saves time, reduces risk, and makes scaling manageable.

---

### **3. Swap Without Breaking (Liskov Substitution Principle)**

Later in the game, you unlock alternate recipes. Maybe copper is scarce, so you switch to an iron recipe for wire. The rest of your factory doesn’t care, it still gets wire, and production flows on.

That’s the **Liskov Substitution Principle**: one component can be replaced by another without breaking the system. The abstraction (“wire”) remains intact, even if the underlying implementation changes.

---

### **4. Clean Contracts (Interface Segregation Principle)**

Early on, you power machines with leaves and wood in a bio burner. Later, you move to coal, oil, or even nuclear. The generators get more complex, but the wires stay the same.

Machines don’t care where the electricity comes from, they just need power. That’s **Interface Segregation**: keep interfaces small and focused so consumers only depend on what they actually use. By keeping the “contract” simple, you can swap implementations freely without chaos.

---

### **5. Design Around Abstractions (Dependency Inversion Principle)**

Think about a motor factory. In the early game, it’s messy and inefficient, but it works. Later, you rebuild it with better layout and throughput. To the rest of your factory, nothing changes, it still receives a steady flow of motors.

That’s the **Dependency Inversion Principle**: high-level modules depend on abstractions, not low-level details. Other parts of your system rely on “motors,” not the exact design of your factory. By designing around abstractions, you can swap or improve implementations without breaking the wider supply chain.

---

### **Final Thoughts**

This started as a fun reflection while playing, but it really made me think about coding habits too. *Satisfactory* may just be a game, but the way it mirrors SOLID principles offers a fresh perspective on software design.

Hopefully, it gives you some new ideas or at least a little entertainment, the next time you’re building something, in a game or in code.

---

### **Extra Resources**

- [SOLID Principles explained in simple terms - DEV.to](https://dev.to/mstuttgart/understanding-solid-principles-a-beginners-guide-4fl6)
- [Satisfactory](https://www.satisfactorygame.com/)