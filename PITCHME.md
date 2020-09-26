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

```js
function SinglyLinkedList() {
  let head = null;
  let length = 0;

  const isEmpty = function () {
    return length === 0;
  };

  const append = function (value) {
    const node = Node(value);
    if (isEmpty()) {
      head = node;
    } else {
      let tempNode = head;
      while (tempNode.next) {
        tempNode = tempNode.next;
      }
      tempNode.next = node;
    }
    length++;
  };

  const prepend = function (value) {
    const node = Node(value);
    if (isEmpty()) {
      head = node;
    } else {
      let secondNode = head;
      head = node;
      head.next = secondNode;
    }
    length++;
  };

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

  const showList = function () {
    if (isEmpty()) {
      console.log("Empty list");
    } else {
      let lists = [];
      let tempNode = head;
      while (tempNode) {
        lists.push(tempNode.value);
        tempNode = tempNode.next;
      }
      console.log(lists.join(" -> "));
      }
  };

  const showLength = function () {
    console.log("length : ", length);
  };

  const deleteAtIndex = function (index) {
    if (isEmpty() || index < 0 || index > length - 1) {
      console.log("Lists is empty or invalid index");
    } else {
      if (index === 0) {
        head = head.next;
        length--;
      } else {
        let previousNode;
        let currentNode = head;
        let counter = 0;
        while (counter < index) {
          previousNode = currentNode;
          currentNode = currentNode.next;
          counter++;
        }
        previousNode.next = currentNode.next;
        length--;
      }
      showList();
    }
  };

  const deleteAtValue = function (value) {
    if (isEmpty()) {
      return null;
    } else {
      let previous;
      let nodetoDelete = head;
      let counter = 0;
      while (counter < length && nodetoDelete.value !== value) {
        previous = nodetoDelete;
        nodetoDelete = nodetoDelete.next;
        counter++;
      }
      // value not found
      if (counter === length) return null;
      if (counter === 0) {
        head = head.next;
      } else {
        previous.next = nodetoDelete.next;
      }      
      length--;
    }
    showList();
  };

  return {
    append,
    prepend,
    deleteAtValue,
    deleteAtIndex,
    insertValueAtIndex,
    showList,
    showLength
  };
}
```

@snap[east span-50 text-blue text-08]
@[1-50](You can step-and-ZOOM into fenced-code blocks, source files, and Github GIST.)
@[50-100, zoom-12](Using GitPitch live code presenting with optional annotations.)
@[100-131, zoom-12](This means no more switching between your slide deck and IDE on stage.)
@snapend

+++?image=assets/img/code.jpg&opacity=60&position=left&size=45% 100%

@snap[east span-50 text-center]
## Now It's **Your** Turn
@snapend

@snap[south-east span-50 text-center text-06]
[Download GitPitch Desktop @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend

