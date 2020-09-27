# Ready, Get set, ... **GO**

+++

@css[text-blue fragment](Hello, World!)

+++

@box[text-orange span-80 fragment](Mars Attacks # Greetings earthlings. We come in peace!)

+++

@snap[west]
## Hello
@snapend

@snap[east fragment]
## Martians!
@snapend

+++

@fa[smile-o fa-4x fa-spin fragment]

+++

### Add Some Slide Candy

![IMAGE](assets/img/presentation.png)

+++?color=linear-gradient(180deg, white 75%, black 25%)
@title[Customize Slide Layout]

@snap[west span-55]
## Customize the Layout
@snapend

@snap[north-east span-45]
![IMAGE](assets/img/presentation.png)
@snapend

@snap[south span-100]
Snap Layouts let you create custom slide designs directly within your markdown.
@snapend

+++
@title[Add A Little Imagination]

@snap[north-west span-50 text-center]
#### Engage your Audience
@snapend

@snap[west span-55]
@ul[list-spaced-bullets text-09]
- You will be amazed
- What you can achieve
- With a **little imagination**
- And GitPitch Markdown
@ulend
@snapend

@snap[east span-45]
![IMAGE](assets/img/conference.png)
@snapend

@snap[south span-100 bg-black fragment]
@img[shadow](assets/img/conference.png)
@snapend

+++?color=linear-gradient(180deg, white 50%, #005f6b 50%)
+++?gist=gitSushi/6e80057358793b4ab282d7adb68d1171

@snap[north span-100 h3-pink]
### The details of the code
@snapend

@snap[south span-100 text-purple text-10]
@[1-6](Instead of using a class which is essentially a function returning an object, we will do just that to declare our function *Node*.)
@[8-10](*SinglyLinkedList* will be the outer function of our closures. Initialization of the two variables that we need to keep track of: *head* and *length* of the list.)
@[12-14](A helper function that returns a boolean wether the list empty or not.)
@[16-28](append)
@[30-40](prepend)
@[42,](Declare the insertValueAtIndex with its two parameter, value, index.)
@[43-44](If the index is out of bounds log "Invalid index".)
@[45-47](Call the prepend function if the index is 0.)
@[48-52](Knowing the index is valid, initialize the necessary variables to insert the new node. The *previousNode* will allow to point at the new node which will point at the *currentNode*.)
@[53-57](Iterate till the index is found which sets the variables.)
@[58-63](Finally add the new node by referencing the pointers. Finally increment length.)
@snapend

+++?image=assets/img/code.jpg&opacity=60&position=left&size=45% 100%

@snap[east span-50 text-center]
## Now It's **Your** Turn
@snapend

@snap[south-east span-50 text-center text-06]
[Download GitPitch Desktop @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend

