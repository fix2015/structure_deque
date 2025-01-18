# Deque Data Structure in JavaScript 🚀  

A simple implementation of the **Deque** (Double-Ended Queue) data structure in JavaScript. This repository demonstrates how to create a deque class with essential methods and explains its functionality with practical examples.  

---

## What is a Deque?  
A **Deque** (Double-Ended Queue) is a linear data structure that allows elements to be added or removed from both ends—front and back. It is a generalization of a queue, where elements can be inserted or removed from either end, making it more versatile than a standard queue.  

---

## Features  
- **InsertFront**: Add an element to the front of the deque.  
- **InsertBack**: Add an element to the back of the deque.  
- **RemoveFront**: Remove and return the element from the front.  
- **RemoveBack**: Remove and return the element from the back.  
- **PeekFront**: View the element at the front without removing it.  
- **PeekBack**: View the element at the back without removing it.  
- **Size**: Get the number of elements in the deque.  
- **isEmpty**: Check if the deque is empty.  

---

## Code Implementation  

Here’s the JavaScript implementation of the deque:  

```javascript
class Deque {
    constructor() {
        this.items = [];
    }

    // Add an element to the front of the deque
    insertFront(element) {
        this.items.unshift(element);
    }

    // Add an element to the back of the deque
    insertBack(element) {
        this.items.push(element);
    }

    // Remove and return the element from the front of the deque
    removeFront() {
        if (this.isEmpty()) {
            return "Deque is empty!";
        }
        return this.items.shift();
    }

    // Remove and return the element from the back of the deque
    removeBack() {
        if (this.isEmpty()) {
            return "Deque is empty!";
        }
        return this.items.pop();
    }

    // Peek at the element at the front without removing it
    peekFront() {
        if (this.isEmpty()) {
            return "Deque is empty!";
        }
        return this.items[0];
    }

    // Peek at the element at the back without removing it
    peekBack() {
        if (this.isEmpty()) {
            return "Deque is empty!";
        }
        return this.items[this.items.length - 1];
    }

    // Get the size of the deque
    size() {
        return this.items.length;
    }

    // Check if the deque is empty
    isEmpty() {
        return this.items.length === 0;
    }
}
```

---

## Example Usage  

```javascript
// Initialize the deque
const deque = new Deque();

// Insert elements at the front and back
deque.insertFront(10);
deque.insertBack(20);
deque.insertFront(5);

// Peek at the front and back elements
console.log(deque.peekFront()); // Output: 5
console.log(deque.peekBack());  // Output: 20

// Remove elements from the front and back
console.log(deque.removeFront()); // Output: 5
console.log(deque.removeBack());  // Output: 20

// Get the size of the deque
console.log(deque.size()); // Output: 1

// Check if the deque is empty
console.log(deque.isEmpty()); // Output: false
```

---

## Real-World Applications  
1. **Task Scheduling**: Used in round-robin scheduling for managing tasks.  
2. **Sliding Window Algorithms**: Efficiently processing a range of elements in an array or list.  
3. **Palindrome Checker**: Checking if a string is a palindrome by comparing characters from both ends.  
4. **Deque-based Buffer**: Implementing a buffer where data can be inserted and removed from both ends.  

---

## TikTok Tutorial 🎥  
Want to see a quick tutorial on how to build this? Check out this TikTok video:  
[]()  

---

## How to Run the Code  
1. Clone the repository:  
   ```bash
   git clone https://github.com/fix2015/structure_deque
   cd structure_deque
   ```
2. Open the file `index.js` in your favorite code editor.  
3. Run the file using Node.js:  
   ```bash
   node index.js
   ```

---

## Contributing  
Contributions are welcome! If you have suggestions or want to add new features, feel free to create a pull request.  

---

## License  
This project is licensed under the MIT License.  

---

## Connect with Me:
- [LinkedIn - Vitalii Semianchuk](https://www.linkedin.com/in/vitalii-semianchuk-9812a786/)
- [Telegram - @jsmentorfree](https://t.me/jsmentorfree) - We do a lot of free teaching on this channel! Join us to learn and grow in web development.
- [Tiktok - @jsmentoring](https://www.tiktok.com/@jsmentoring) Everyday new videos
- [Youtube - @jsmentor-uk](https://www.youtube.com/@jsmentor-uk) Mentor live streams
- [Dev.to - fix2015](https://dev.to/fix2015) Javascript featured, live, experience but about Deque
