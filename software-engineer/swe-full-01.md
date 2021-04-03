# Fullstack Software Engineer

- You are required to implement REST endpoint `GET /product/search` that basiclly accept user's search query and searches available products by name.
- Endpoint should return back as JSON response a list of matched products along with products' current lowest price. please check below for suggest response.
- In order to search product's name, we implemented [external service](), it searches product by name, manufactureres and trademark and return list of matched products, retrived details include product's unique identifier, name, manufacturer, image and some other display purpose details.
- Once you receive matched products' list, you should lookup retrived product's availablity and prices in local relational database of your choice and design.
- Local database should store product's availabilty status for every seller available on the system, in addition to product's price and any available offers, in addition to whatever you think should be stored.
- Additionally with VueJS implement a Search dropdown component as a Vue Component that uses the endpoint you created to search products, and lists search results in dropdown.
- Implemented component should be generic and configurable so it is able to work with your created endpoint or other endpoints.
- Component design should be responsive, so it adapts on surrounding display area, and results in drop down area should not get messy on small devices.

### Endpoint Parameters
 - `q` search parameter (string)
 - `page` for pagination
 - `fields` comma separated list of additional fields
     - `price`
     - `sellers`
   
#### Suggested response
```json
{
    "data": [
        {
            "product_id": 1001,
            "name": "منتج غذائي",
            "price": 50, // optional if `price` passed in query parameter `fields`
            "seller_count": 3  // optional if `sellers` passed in query parameter `fields`,
        }
    ],
    "meta": {
        next: 2,
        prev: 0
    }
}
```


We love documentations, at all levels, also we love git, so always deliver you code
in a git repo, with readme.md file descriping how should we get your
code working, you may also include:

- Your thinking process, how you designed your solution.
- Any Diagrams, System diagram, ERD, Draft Drawing, UI Mocks … you may mobile photo and send it in.
- Any leftouts? what you may added if you got additional time.
- Tell us about something you learned during the coarse of this task.
- Useful link(s) related to you or the task you may like to share with us.

# How We Evaluate

We love pefection, therefore, deliver **_quality_** task instead of _complete_ task, make sure your
code is production ready, this matter.

- **Simplicty**, write simple, clean code, Complexity is Human Programmer's Enemy
- **Correctness**, always focus on what output we asked for in the task
- **Security**, no one loves to be vulnerable, so we are
- **Testing**, we care about testing, very much
- **Documentation**, we love documentation, provide as much documetation as you can.
