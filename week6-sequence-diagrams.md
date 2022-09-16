# Week 6: Interpreting UML sequence diagrams

Tags: `W6` `UML diagrams` `sequence diagram`

# Q&As

**Q: Is it correct to interpret that the `main` method calls the `producePrototype()` method of m?**

**A:** No. We do not know who is calling the `producePrototype` since it is not specified in the diagram. 

The precise way of describing this should be: an *unspecified object* calls the `producePrototype()` method of m.

**❌ Common misconception:** The `main ` method calls the `producePrototype()` method.

**Q: Are there any differences between the first and second activation bar?**

**A:** Yes. The first one is attached to the box, representing a constructor of a class. 

The second one is just a normal activation bar. 

They both represent something being activated though.

**❌ Common misconception:** No difference, just one is called before the other.

**Q: Does italics in sequence diagram represent abstact method?**

**A:** No. Italics does not mean anything in sequence diagram. It does not represent *abstract method*. 

Italics does represent abstract method in *class diagram* though. You can revise your *class diagram* here.

**❌ Common misconception:** It represents *abstract method*.

**Q: Is it OK to omit the *return arrow*?**

**A:** Yes. It does not affect anything, and does not change the meaning of the diagram. The *return arrow* is optional in sequence diagram.

**❌ Common misconception:** Omitting means the method does not return anything. 

**Q: If we omit the return arrow, does it mean that `stressTest()` method return nothing?**

**A:** We do not know. Since nothing is being written at the return arrow, it could be that it is retuning something, or it could be that it does not return anything.

**Q: So since in this case we have a return arrow, does it mean that the `stressTest()` method return something?**

**A:** Same answer as above.

**❌ Common misconception:** Return arrow *must* mean the method is retuning something.

**Q: In the sequence diagram, for any void type of method, can we use a return arrow?**

**A:** Yes.

**Q: In this diagram, the return arrow at the bottom shows which value will be returned. In this case, is the return arrow omittable?**

**A:** No. As the text is an add-on to the arrow, the text should not appear without the arrow.

- Omit everything: OK
- Show arrow only: OK
- Show arrow and text: OK
- Show text but not arrow: not OK


# Noteworthy
- In UML diagrams, many things are *optional*. Just because the diagram does not show something does not mean that those things do not exist. It just means that who ever drew the diagram was not interested in showing all those details that have been omitted because they may not be relevant for the purpose of the diagram.

- Time travels from top to bottom in the sequence diagram.

# Something to think about

These are something that you could try to think about when you are revising this topic. Feel free to discuss with your team/forum/me if you are not sure 😄

1. Other than the *abstract method* is there any other differences between how things are represent in sequence diagram and other UML diagrams (e.g. object/class diagram)?

# Interesting forum discussions
Seems like there is not much discussion on sequence diagram in the forum as of now. Will add to the list if I see interesting stuff!