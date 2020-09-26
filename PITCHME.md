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

+++

@snap[north-east span-100 text-pink text-06]
Let your code do the talking!
@snapend

```js zoom-8
  const insertValueAtIndex = function (value, index) {
    if (index < 0 || index > length) {
      console.log("Invalid index");
    } else {
      if (index === 0) {
        prepend(value);
      } else {
        const node = Node(value);
        let previousNode;
        let currentNode = head;
        let counter = 0;
        while (counter < index) {
          previousNode = currentNode;
          currentNode = currentNode.next;
          counter++;
        }
        previousNode.next = node;
        node.next = currentNode;
        length++;
      }
    }
  };
```

@snap[south span-100 text-blue text-10]
@[1-4](You can step-and-ZOOM into fenced-code blocks, source files, and Github GIST.)
@[4-7, zoom-8](Using GitPitch live code presenting with optional annotations.)
@[7-16, zoom-16](This means no more switching between your slide deck and IDE on stage.)
@snapend

+++?image=assets/img/code.jpg&opacity=60&position=left&size=45% 100%

@snap[east span-50 text-center]
## Now It's **Your** Turn
@snapend

@snap[south-east span-50 text-center text-06]
[Download GitPitch Desktop @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend

