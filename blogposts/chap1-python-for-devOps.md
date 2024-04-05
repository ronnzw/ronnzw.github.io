# Python for DevOps
A the time of writing this article l'm reading a book called Python for DevOps O'reilly. I will be summarizing each chapter as l go through the book. Ofcourse my summary won't be a summary about the particular chapter but a summary of what l found to be interesting, hopefully it will be interesting to you as well. Ok enough talking let's get into it.

## What is DevOps
The writers understood that devOps means different things to different people so the writers have identified evidence that there is DevOps and here is a list of what they have said.

### List of evidence of DevOps
- Two-way collaboration between Development and Operation teams.
- Turnaround of Ops tasks in minutes to hours, not days to weeks.
- Strong involvement from developers; otherwise, it’s back to Devs versus Ops.
- Operations people need development skills—at least Bash and Python.
- Developer people need operational skills—their responsibilities don’t end with writing the code, but with deploying the system to production and monitoring alerts.
- Automation, automation, automation: you can’t accurately automate without Dev skills, and you can’t correctly automate without Ops skills
- Ideally: self-service for developers, at least in terms of deploying code.
- Can be achieved via CI/CD pipelines
- GitOps.
- Bidirectional everything between Development and Operations (tooling, knowledge, etc.).
- Constant collaboration in design, implementation, deployment—and yes, automation—can’t be successful without cooperation.
- If it isn’t automated, it’s broken.
- Cultural: Hierarchy < Process.
- Microservices > Monolithic.
- The continuous deployment system is the heart and soul of the software team.
- There are no superheroes.
- Continuous delivery isn’t an option; it is a mandate.

### What l think about DevOps
DevOps for **me** is a methodology to deliver value to the consumer/customer in the shortest possible time. This was also the view of my last employer. Hence it is characterised by things like automation, continuosly development, continuosly integration and delivery. So l agree with most of the things that the writers used to describe evidence of DevOps. 


## Ipython
IPython provides a rich architecture for interactive computing besides the built-in interactive shell. IPython
offers introspection (the ability to dynamically get information about objects), syntax highlighting, special magic commands. It is most useful if you want to see and use things under the hood.

One can easy install Ipython using pip.
`pip install ipython`

running it is as simple as running is similar to running the built-in interactive shell described
in the previous section:
```bash
ipython
```

### Using Ipython to run shell commands
One can run shell commands using ipython. Let’s take a look at a very simple example where the `!` character, which IPython uses to identify shell commands.
Bash: `ls`
IPython: `!ls`

The commands' output can be assigned to a variable. If you check the type of a variable its `IPython.utils.text.SList` thus a regular command has been converted to be an object. You can perform operations like `sort`, `grep` and `field`.

```bash
ls_variable = !ls
ls.variable.sort(2,nums = True)
```
This will sort the second column

### IPython magic commands
Just like there previous commands that l showed you. There are others that are called **magic** commands. To use a magic commands you need to use `%%`. Ro running bash commands with the magic commands you would simply same.
```bash
%%bash
ls
```
Boom again you are running commands in the interactive shell. You are also write files using `%%writefile name_of_file.py` the specify the content to write.

# Conclusion
IPython is a nice why of interacting with commands within the shell. You can also save these commands as object that you can play around with. I can definately see this being handy in the coming chapter as well as into DevOps. For me it's the first time interacting with IPython but l have immediately fallen in love with it.