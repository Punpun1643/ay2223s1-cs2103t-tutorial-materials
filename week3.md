# Week 3: Coding Standards

Tags: `W3` `coding standard`

# IMPORTANT: update on coding standard

![913D5168-3C77-40BA-A057-01AC604D0131](https://user-images.githubusercontent.com/60144099/187239008-a71aa75b-8297-4b2a-92c3-3a875b5e0cc2.jpeg)

# Q&As

**Q: (Line 7) Must we give an access modifier?**  

```java
List<String> pastDescription = new ArrayList<>(); // a list of past descriptions
```

**A:** The coding standard does not require it. In any case, not having an access modifier is a legit choice in Java (it is called *private package* access). So, if that is the appropriate access level, it is fine to not have an access modifier. 

**Q: (Line 7) Is having comment at the end of the line ok?**

```java
List<String> pastDescription = new ArrayList<>(); // a list of past descriptions
```

**A:** It is fine to have a comment at the end of the line. But when the comment is put above a statement, it should be indented to match the statement. The coding standard disallows comments with mismatching indentation, but does not mention/disallow end-of-line comment. 

**Q: (Line 22) Can we omit javadoc for overridden methods?**

```java
@Override
public String toString() { return descriptionPrefix + description; }
```

**A:** No. The *‘must have x’* rule applies for all cases except for those cases that are explicitly mentioned as *‘can omit for cases…’* Java has a way to specify that a method inherits the comment from the parent class *({@inheritdoc})*, which means there is no need to duplicate the comment in all child classes. 

# Noteworthy

- Some IDEs will use wildcard import if there are more than a certain number of classes from the same package. This is against our coding standard.

- Although coding standard doesn’t specifically say parameter names should not be single letters, it mentions that scratch variables can be single letters. It is OK if someone interprets this as other names should not be single letters.
 
```java
public Task(String d) {
    ...
}
``` 

- The coding standard says ‘this.’ should not be used unless necessary. But that is an advanced rule (optional to follow). Only basic and intermediate level guidelines are applicable to the module.
    
```java
this.important = true
```
    
- The style in `DESCRIPTION_PREFIX` (i.e. all capitals, separated by underscores) is sometimes called *screaming snake* style
