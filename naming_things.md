---
marp: true
theme: uncover
backgroundColor: #123
color: #fff

---

# Nicolai Gjellestad

### Developer at Nicode and Ilder
![Ilder width:300px height:auto](./assets/ilder.svg)
<!---
- Developer from Bergen
- Work at my own company Nicode
- Work on cool and sustainable projects with Ilder
--->

---
## Solving the hardest problem in programming
### Naming things :tada:
<!---
- It's a joke, but also kind of true
- I've seen a lot of bad naming through the years
- My goal is giving you a framework to improve naming
--->
---
# Why is it even a problem? 
# :thinking:
<!---
- We don't prioritize it
- We forget that others should understand this
- Tests run, compiles, nothing more needs to be done
- We forget that code is read more than it's written
- It's important that team mates understand each other
- A bad name can be the difference between clear and cryptic code
--->
---
# Code is communication
# 🤓
<!---
- The code we write describes how it works and what it represents to other humans
- Most of us don't think about code as communication, but it really is
- The audience is your team, client or all developers in the world
- I like to think about code as I think of writing
- Take the analogy further, I like to cook and I like to write a cookbook
--->
---
- 2 e
- 4 dl m
- 350 g f
- 100 g s
<!---
- My first version
- I understand everything, I wrote it! 
- My editor don't understand anything
- What are we making?
--->

---
# Waffle recipe 🧇
- 2 e
- 4 dl m
- 350 g f
- 100 g s
<!---
- I added a title
- Everything should be clear now
- As a programmer I like the short names, it's efficient
- Editor still isn't happy
- Don't expect your readers to decode the ingredient list
- Ingredient names must be specific
--->
 
---
# Waffle recipe 🧇
- 2 ovum of gallus domesticus
- 4 dl milk from bos taurus
- 350 g ground and sifted triticum aestivum
- 100 g sucrose
<!---
- Now things are super specific
- Scientific names all over the place
- My editor is frustrated. 
- Readers heads will explode reading this
--->

---
# Waffle recipe 🧇
- 2 eggs
- 4 dl milk
- 350 g flour 
- 100 g sugar
<!---
- Perfect
- Now everything makes sense, easy to read and comprehend
- Editor is happy
- I've written a recipe for a target audience
--->

---
# Context
- Packages
- Functions
- Loops
- Data structures
<!---
- Context is like the title of the recipe
- Gives the reader a mental model to understand the text/code
- Stronger context is more understandable.
- Stronger context let's you have short and consice names
- Datamodel Car, have a property Engine
- Car is the context engine lives in
- If Engine was outside the context it would have to be more verbose
- Car engine
--->

---
![bg](#fff)

✅
```go
package users

func New() User {
}
```
❌
```go
package utils

func New() Padder {
}
```
<!---
- The function name New in package user makes total sense
- It's short and clear because it delivers a user and lives in the user package
- New in package utils doesn't make sense. 
- What do it do? What's a util? 
--->
---
# Verbosity
- r
- repo
- userRepo
- userRepositoryLayer
<!---
- These are all different verbosity levels of the same concept
- The context decides the level of verbosity
- One letter variables is fine, as long as the context allow it
--->
---
# Think like an editor 🤓 📖
<!---
- Write code for an audience
- How will they read and interpret the code? 
- Code will never be perfect in the first try
- See your code from an outside perspective
- Iterations, restructuring and renaming will improve the code. 
- How does it fit in the bigger story == codebase ? 
--->