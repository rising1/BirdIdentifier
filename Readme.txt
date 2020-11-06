This file keeps the notes to get the cloud platform up and running

pip3 install  -r requirements.txt - ********************* not needed
sudo apt-get install google-cloud-sdk-app-engine-python - ******** not needed
gcloud components install app-engine-python -***************** needed
cd c:\users\phfro\PycharmProjects\Starter ************** needed
gcloud components install alpha ***************** installs billing for projects
gcloud alpha billing accounts list ******** lists billing accounts
gcloud alpha billing projects link rising1-starterworking --billing-account 014D72-568206-2FA7E1
gcloud projects create rising1-starterworking --set-as-default
gcloud services enable cloudbuild.googleapis.com
gcloud app create --project=rising1-starterworking
gcloud app deploy

gcloud app versions stop 20201031t160121

gcloud projects list
gcloud config set project


to tail the logs

gcloud app logs tail