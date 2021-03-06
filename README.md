# best-programming-club-2020-12-20

## User Interface

![User Interface Mock up of the detailed shopping cart and product list. It looks a bit minimalistic with cheerful color scheme of orange, greyish brown, lime green, pink and mostly white. It looks pretty cute.](/img/cart_mockup.png "Current mock up of the online farmers' market and detailed cart view.")

I was going for an online farmers market page, geared towards a younger demographic. Inspired by Animal Crossing, Cooking Mama, but not too cheeky. I used [Adobe Color](https://color.adobe.com/create/color-wheel) to get a color scheme for this.

*I took photographs of produce and basket icon from the internet. Refer to the sources at the bottom of this page for credits. 

## Kim's BYO-Assignment: Add Detailed Cart View ##

I wanted to display what was inside the cart, by listing how many of each products were chosen.

First, There is a `count` key in each product object in `itemsInCart`. As each product is added, the count goes up. So `itemsInCart` is no longer a list of objects that are sometimes multiples of the same, as we select multiple of one type of product. It is now a short list with each objects its own counter. 

To add a prodcut to `itemsInCart`, check if the cart is empty. If it's not empty, then check if the selected product's type already exists in `itemsInCart` using a for loop. If we determine this is a new product, then we'll add a new product object. I keep track of all these different conditions with a boolean variable, `isInCart`.

<!-- Before going into datails of adding products to `itemsInCart`, there is a boolean variable `isInCart`. It shows whether the selected product has been counted. This will become helpful in keeping track when we are determing if the selected product's type already exists in `itemsInCart` or not. 

To add a product to
 `itemsInCart`, we first need to check if the cart is empty. If it is, then we add a new product object to `itemsInCart`, with initial `count: 1`. We also set `isInCart = true`. If it's not empty, then we start checking if each of the existing product matches with the selected. We do this with a for loop, that will initially set out to look through every single object, but it'll break if we find the matching product. If we find the matching product, we only increment the `count` key 

To add a prodcut to `itemsInCart`, we need to check if the cart is empty.
If it's not empty, then check if the selected product's type already exists in the cart. If we determine this is a new product, then we'll add a new product object. I keep track of all these different conditions with a boolean variable, `isInCart`.


When a button is clicked, it is automatically set to false. It'll increment itself when we either add the product object to `itemsInCart` or increment one of the existing product object. -->

### Challenges and shit ###

1. The biggest challenge was checking if the selected product already exists then adding the product accordingly. I kept getting stuck in a for loop. Having a boolean checker fixed my problem. 

2. I kept getting the HTML display of `itemsInCart` repeated every time a button was clicked. I ended up resetting and displaying the updated `itemsInCart` per button click. 

## Assignment

1. BYO-Assignment: Add a new feature to the Farmer's Market shop that would improve the user experience.
2. Come up with a nicer user interface design (in an Adobe program, [Figma](https://www.figma.com/), [Sketch](https://www.sketch.com/), etc) and add a screenshot of it to this README (See [GitHub guide on images in Markdown](https://guides.github.com/features/mastering-markdown/).)

### Getting the assignment

[Fork this repository](https://guides.github.com/activities/forking/)

[Install Prettier for VSCode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

### Completing the assignment

Make sure to commit your changes as you're making progress on the assignment. You'll receive feedback on the commit messages. Remember, commit messages should be short and sweet, in present-tense with an imperative tone. For example:

```
rename cart variable
```

### Remember...

- Actively ask the Discord channels for help!
- Google as much as you can, using the keywords you've learned. For example, search _"how to create HTML from javascript"_ or _"what is javascript forEach"_ or _"what is javascript dataset"_. MDN is a great keyword to include in your searches for reference materal, for example _"MDN javascript array"_.
- Don't be afraid to commit code that's not working yet.

#### Sources for photographs

[Add to Cart Icon](https://www.rawshorts.com/freeicons/?download=add-to-cart-icon)

[Apple](https://fineartamerica.com/featured/apples-for-sale-at-a-farmers-market-edwin-remsberg.html)

[Banana](https://www.pinterest.com/pin/858991328906408783/)

[Broccoli](https://www.thespruceeats.com/all-about-broccoli-2215869)

[Squash](https://www.wideopeneats.com/summer-squash/)

[Carrots](https://www.encirclephotos.com/image/multi-color-carrots-at-farmers-market-in-vancouver-canada/)

