# Day 5 Lessons

## Challenge

- This may be rather heavy for you today. We're going to practice it now by creating `CommentsController` and all it's associated methods

- Refer to yesterday's lessons and today's (It is principally similar to `Topics and Posts`, now you are just building one nest deeper for `Comments`)

- Be wary that it is now 2 levels deep for your comments. Be sure to pass in both the id of `topic` and `post` into your urls when creating for `comments`.

- A hint to get you started, in your `routes.rb`:

  ```
    resources :topics, except: [:show] do
      resources :posts, except: [:show] do
        resources :comments, except: [:show]
      end
    end
  ```
