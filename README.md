# fastai-gcp-manager
A simple GCP management CLI for FastAI training.

**Commands:**
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
