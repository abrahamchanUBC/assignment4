# Assignment 4

This is a continuation of [Assignment 3](https://github.com/erkartik91/assignment3). As a part of this assignment, you will focus on interacting with the remote server to fetch the product items.

## Tasks

1. **Fetch products from server using AJAX:** You will initialize your **product** variable by making an ajax call to the following url and **cart** variables will be initialized empty like the previous assignment. 
  ```
  https://cpen400a.herokuapp.com/products
  
  var cart = {
    'productName1' : 0,
    'productName2' : 0,
    ...
  };
  ```
  You **do not** need to keep price information in the cart as that information is already there in the products array. When calculcating the total price of the products in cart, you can use the price information from the products array. Please feel free to assign prices to products as you like.

2. **Handle Timeout / Error:** The remote server you are fetching the data from is not very reliable. Sometimes, instead of returning the product list the server takes long time, due to which the ajax request times out. Also, sometimes the server returns error 500 instead of the product list. In either case you will need to make another AJAX call untill you get the list of products from the web server.

3. **Synch up price / quantity before checkout:** In your show cart modal you need to present the user with a checkout button. When the user clicks on checkout, you will need to make sure that the products are still available in the back store and the prices are updated. You will do that by making another AJAX call to the same url. Therefore, when the user clicks on checkout, you will alert the user with the message showing that your are confirming the final total price as well as the availability.  If there is any price change, you will need to alert the user for each product for which the price changed. In case for any produt, quantity that the user ordered is not available any more, you will change the number of products in the cart to the new available quantity. You will also need to alert the user about the updated quantity as well. The cart variable should also be updated the reflect the new prices/quantity.

4. **Update Cart modal and show total price:** Once you have the updated cart information, you will need to update the relevant cart information shown to the user. Also, you will alert the uset with the total amount due.

## Submission instructions:

* Add a folder called **assignment4** in your github repo.
* Copy the code from your assignment3
* Update the code to reflect the changes for this assignment.
* Make sure you push your changes before midnight (11:59 PM) before the day when assignment is due - late submissions will not be accepted.
* We will be downloading the code on the midnight before the due date, any changes to code after that point will not be considered for marking.
