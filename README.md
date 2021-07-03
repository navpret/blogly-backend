# Blogly

An application that allows anyone to post blogs. This is the backend repository for the application, which is an API.

# How to setup

1. Clone the repo in the usual way, then `cd` to the directory

1. Create a `.env` file in the project root, and add the following entries:

```config
PORT = 4040
MONGO_URL = <YOUR_MONGODB_HOSTED_URL>
```

If you are the marking professor, contact me through teams or mail, and I'd be on top of this world to provide you my mongodb url containing pre-made blogs

1. Install all dependencies by running

```bash
npm install
```

1. Run the application using:

```bash
npm start
```

This would run the server on port provided in the `.env` file

# Why is the repo created late

The previous repo had been created way before this one. Howvwer, I got a mail from some sort of credential-breach bot that notified me that my mongo-db url had been left inside this repo. On checking I found out that I forgot to add the `.env` file to `.gitignore`, which lead to my mongodb username and passwords being publically available. Therefore, I had to make that repository private, making it very hard to get hold of the credentials. Therefore, I created this repository again.

If you are the professor and still need to see that repository, Alix still has access to that repo, since he had been invited before the privatizing the repo. If you would check your mail, you'd find the invite, and would be able to view that part. However, all new work has been updated in this repo, and that one is still not being maintained.

# How to use the API

This is the repo for the REST API created using NodeJS and ExpressJS to serve the Blogly frontend and it could be access through [this URL](http://143.244.136.44:4040/), and this version is also deployed on the mi-linux server, and could be accessed using this command, while SSH into the mi-linux.wlv.ac.uk sercer

```bash
curl http://mi-linux.wlv.ac.uk:4040
```

Though this could be accessed from inside, it is still not accessible through the internet, since opening ports on the mi-linux server requires sudo access, which the students don't have. Thus, the frontend uses that URL in order to communicate.

### Thank You
