# test pollination apps

testing...

## Quickstart

Install dependencies:

```
> pip install -r requirements.txt
```

Start Streamlit

```
> streamlit run app.py

  You can now view your Streamlit app in your browser.

  Network URL: http://172.17.0.2:8501
  External URL: http://152.37.119.122:8501

```

Make changes to your app in the `app.py` file.

## Run inside Docker image locally (Optional)
You can run the app locally inside Docker to ensure the app will work fine after the
deployment.

You need to install Docker on your machine in order to be able to run this command

```
> pollination-apps run <app folder> devang --name "test pollination apps"
```

## Push to Pollination
Push you app to pollination to share it with others.

Login to pollination:

```
> pollination-apps login
```

Deploy your app to pollination:

```
> pollination-apps deploy . --name "test pollination apps" --public
```


## Configure Github Actions

In order to configure github actions to deploy your app you will need to:

1. Configure a secret called `POLLINATION_TOKEN` with your Pollination API key as the value
2. Create [a new release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository) of your app on Github with a new tag

Github actions will then package and deploy your code to an app called [test pollination apps](https://app.pollination.cloud/devang/applications/test pollination apps)


