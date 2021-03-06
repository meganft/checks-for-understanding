## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?<br>
`rails new project-name` 

2. What do Models generally inherit from in rails?<br>
`ActiveRecord::Base`

3. What do Controllers generally inherit from in a rails project?<br>
`ApplicationController`

4. How would I create a route if I wanted to see a specific horse in my routes file assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?<br>
`resources :horses, only: [:show]`

5. What rake task is useful when looking at routes, and what information does it give you?<br>
`rake routes`. It shows you all current routes available in your rails app.

6. What is an example of a route helper? When would you use them?<br>
A route helper is something like `edit_company_path(company)`. You would use this in your rails app when linking to the page to edit a specific company, in this instance.

7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?<br>
`_url` is an absolute path rather than the relative path we have defined in our application (where we use `_path`). So if we are sending an email or linking to something ourside our app, we use _url.

8. What are strong params and why are the necessary? <br>
Strong params provide us with another level of security from submitted data. We only want to receive the permitted info so we define that in our controller.

9. What role does `form_for` play in helping us create our forms? <br>
It is a rails helper method that caputeres user input data.

10. How does `form_for` know where to submit the user's input? <br>
Based on the variable we passed to it. If it was a form_for @horse, it would know that it was dealing with an instance of a horse.

11. Create a form using a `form_for` helper to create a new `Horse`. <br>
```
<%= form_for (@horse) do |f| %>
  <%= f.label name %>
  <%= f.text_field name %>
  
  <%= f.label age %>
  <%= f.text_field age %>
  
  <%= f.submit %>
<% end %>
```

12. Why do we want to validate our models?<br>
We do this to ensure that the relationships between our tables works correctly.
