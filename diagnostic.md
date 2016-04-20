# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The backend is used to take requests from the client, such as patch, post, get,
destroy, and to carry them out through a series of mechanisms.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
The model fetches data for the controller.
```

Which layer in the MVC pattern communicates with the model?

```bash
The controller communicates with the model.
```

Why don't we use views in our interpretation of the MVC pattern?

```bash
Because they are being phased out and we are creating our own views when we create
our own front ends.
```

What does C.R.U.D stand for?

```bash
Create Read Update Destroy
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
In the model
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
Index, Show, Destroy, Update, Create
```

A user action fires a `GET` request for `person/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```bash
- The request goes through a router where it is passed to the correct controller
  method that can successfully carry out the action.
- This controller then passes it onto the model
- The model actually retrieves that data.
- Either an error or the data is returned to the controller depending on whether
  or not the data was found.
- This is then passed back to the client in some form.
```

What is the command to generate a new rails-api app?

```bash
rails-api new "Enter App name" -T --database=postgresql
```

What is the command to start an instance of a rails server?

```bash
rails s or rails server
```

What are the commands to drop, create and migrate a database? (3 bullet points)

```bash
- rake db:drop
- rake db:create
- rake db:migrate
```

What is the command to scaffold a pet with a name and an age?

```bash
rails-api g scaffold pet name:string age:string
```

List two advantages of using serializers? (2 bullet points)

```bash
- It limits/allows access to only certain information, thus making your data
  more secure
- It also allows you to sure of what data is being shared where so that something 
  unexpected wont happen with your data.
```
