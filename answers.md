# Q0: Why is this error being thrown?
The pokemon model has not been initialized (defined).

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
All the pokemon that appear do not have a trainer. The randomness factor comes from the sample function.

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
button_to sends a request to capture_path which is evaluated to /capture, it sends a request of the type defined by method, in this case patch with
the data specified inside capture_path, in this case id: @pokemon.

# Question 3: What would you name your own Pokemon?
RAILSDECALMON

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed in the trainer for the pokemon. It is ok because the show method gets called when we pass in the single trainer in the table entry.

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
When the form is not completed correctly (The user does not fit the requirements of giving a unique non-nil name) then an error will be produced,
which we get from the error produced by the pokemon on the right hand side of the =. The flsh part will display it.

# Give us feedback on the project and decal below!

# Extra credit: Link your Heroku deployed app
