# Task 1 : Update the list section for Header and Footer

## Expected output

![Expected Output](./Expected%20Output-01/task1Output.png)

## Related Code

Adding 'Hire Me' list item :

```
let ul = document.querySelector('ul'); //selecting the list in header
let li = document.createElement('li'); // creating a new li element to add
li.innerText = 'Hire Me'; // adding text inside li
ul.append(li); // adding li to list
```
Updating list item 'Contact' to 'Projects' :

```
<!-- ul.children can be used to visualize all children-->
ul.children[2].innerText = 'Project'; //update the text
```
Removing the list with logos from 'footer' :

```
const footer = document.querySelector('footer'); //seletcting the entire footer
const logo = document.querySelector('footer>ul'); //selecting the list from footer
footer.removeChild(logo); // removing the list from footer
```
# Task 2 : Update the placeholder text in Search Bar

## Expected output

![Expected Output](./Expected%20Output-01/task2Output.png)
## Related Code

Hidding 'Hire Me' list item :

```
li.style.display = "none";
```
Updating the text in Search Bar placeholder :

```
const input = document.querySelector('input');//selecting input tag
input.placeholder = 'Search My Project' //updating the placeholder value
```

# Task 3 : Update description and change placeholder text in Search Bar to original

## Expected output

![Expected Output](./Expected%20Output-01/task3Output.png)

## Related Code

Updating the text in Search Bar placeholder to original :

```
input.placeholder = 'Search'; //updating the placeholder value
```

Updating the description :
```
const para = document.querySelector('.hero-left-section>p');//selecting the paragraph
para.children; // this is just to visualise the contents in the para not needed will show data for the tags like this: HTMLCollection(5) [span, br, span, br, span]
<!-- 0: span
1: br
2: span
3: br
4: span -->

//selecting the appropriate child from the para to update
para.children[2].innerText = 'an Employee';
para.children[4].innerText = 'iNeuron Intelligence Pvt Ltd.'
'iNeuron Intelligence Pvt Ltd'

```
# Task 4 : Update the portfolio picture

## Expected output

![Expected Output](./Expected%20Output-01/task4Output.png)


## Related Code

```
const image = document.querySelector('.hero-right-section>img');//selecting the image
image.src = "./Avatar.jpg"
```

# Task 5 : Update the portfolio picture

## Expected output

![Expected Output](./Expected%20Output-01/task5Output.png)


## Related Code

```
const button = document.createElement('button');//creating the button
button.innerText= 'Support Me';//adding text for button
const buttonsection = document.querySelector('hero-right-section-btns');//selecting the section to add button
buttonsection.appendChild(button);//adding the button to section
```