# fastai-gcp-manager
A simple GCP management CLI for FastAI training.

Use this script to easily start, stop, connect, or get information about your GCP instance for fast.ai. This script will only work once you have installed and configured your GCP instance using the instructions found here: https://course.fast.ai/start_gcp.html

A simple one line command `fastai start` connects to your instance instantly:
![Screenshot of the program running](https://raw.githubusercontent.com/christianblandford/fastai-gcp-manager/master/fastai-manager-screenshot.PNG)

# Installation:
* Install and configure GCP CLI following the instructions [here](https://course.fast.ai/start_gcp.html)
* Paste the following into your terminal and hit enter: `mkdir -p ~/bin/ && curl -k -L -o ~/bin/fastai https://raw.githubusercontent.com/christianblandford/fastai-gcp-manager/master/fastai && chmod a+x ~/bin/fastai && source ~/.profile`
* Run `fastai config` to configure your instance


# Commands:
* fastai *info*
  * Will show the instance/zone if configured
*fastai *status*
  * Shows the status (running/terminated) of the instance configured
* fastai *config*
  * configure the instance and zone to connect to
* fastai *start*
  * spin up the instance, connect to it via ssh tunnel (run this to get to the training)
* fastai *stop*
  * stop the running instance (do this when done training to avoid wasting money)
* fastai *starti*
  * spin up the instance, don't connect to it
* fastai *connect*
  * connect to the instance (must already be running)
* fastai *reset*
  * reset fastai-mgr config file (do this if you messed up configuration)
