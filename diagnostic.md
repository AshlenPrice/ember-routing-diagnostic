# Ember Routing Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  What are the main task(s) you perform inside the Ember Application Router,
    and what are the main task(s) you perform inside an Ember Route?

    ```md
    <!-- your response here -->
    ```

1.  What is the command to generate a route named `boston` nested under
    `campus`?

    ```md
        ember generate route campus/boston
    ```

1.  Suppose you have a nested route at the URL `/campus/boston`. How would you
    use the `link-to` helper to generate an appropriate link?

    ```md
      {{#link-to 'campus.boston'}}Boston{{/link-to}}
    ```

1.  Explain **at least** two differences between the following two route
    definitions.

    ```js
    this.route('products', function () {
      this.route('product', { path: '/:product_id' }); // <= 👀here
    });

    this.route('product', { path: '/products/:product_id' }); // <= 👀 here
    ```

    ```md
    One of the differences in these routes are is the path, one of them should t

     They are nested urls?
     Honestly not sure how to explain this technically but, it seems that the first route will be represented in the url
     as you would need to enter the product id specifically at the end and its a dynamic route.
      - this dynamic route is good to use with ember data

      The second route can be used with a serializer
    ```

1.  Suppose we have the following route definition:

    ```js
    this.route('movie', { path: '/movies/:movie_id' }); // <= 👀 here
    ```

    If we navigate in the browser to `/movies/123`, how can we reference the
    value `'123'` inside a Route?

    ```md
      I think by using a serializer?

    ```

1.  Inside a template, how do we reference data provided by a Route?

    ```md
    it uses the model method that was defined in the route.
    ```
