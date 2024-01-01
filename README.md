# dziupla-dev
Setting up the development environment is **shockingly uncomplicated**!

### Installations
Start off with installing [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) 
and [Docker](https://docs.docker.com/engine/install/).

### Repositories
For Windows users, I recommend using [github desktop](https://desktop.github.com). It's a simple GUI that makes working with git much easier.

To install the necessary repos, you have to clone them from github. While you can do this any other way, I recommend
using an ssh key. [Here is the instruction to generate it.](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
[And here is one to set it up. ](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
Then, all you have to do is clone the repositories with the commands below.
```bash
git clone git@github.com:dziupla-rental/dziupla-dev.git
git clone git@github.com:dziupla-rental/dziupla-back.git
git clone git@github.com:dziupla-rental/dziupla-app.git
```
#### Make sure to clone them into the same empty directory!
### Deployment
To deploy the development server, first navigate into the **dziupla-dev** folder. From it, run the following command:
```bash
docker-compose up -d
```
There you go! Several docker images will be up and running, you can try and access the server at http://127.0.0.1/