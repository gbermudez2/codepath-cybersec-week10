# codepath-cybersec-week10

1. MHN Admin Deployment
- Using the following command, I was able to create the mhn-admin VM.
- gcloud compute instances create "mhn-admin" ^
	--machine-type "n1-standard-1" ^
	--subnet "default" ^
	--maintenance-policy "MIGRATE" ^
	--tags "mhn-admin" ^
	--image-family "ubuntu-minimal-1804-lts" ^
	--image-project "ubuntu-os-cloud" ^
	--boot-disk-size "10" ^
	--boot-disk-type "pd-standard" ^
	--boot-disk-device-name "mhn-admin"
 ![num1](https://user-images.githubusercontent.com/32963758/164160574-e8db438e-1127-4cb9-8fb3-3f11c85321e5.gif)


2. Dioanaea Honeypot Deployment
- Using the following command, I was able to install Dioanaea.
- wget "http://35.230.94.136/api/script/?text=true&script_id=2" -O deploy.sh && sudo bash deploy.sh http://35.230.94.136 Xd9UHT6F
![num2](https://user-images.githubusercontent.com/32963758/164160297-21e92c50-fb65-49ed-a38d-be3bc7f2103a.gif)

3. Database Backup
- Using the following command, I was able to paste the session.json file.
- gcloud compute scp mhn-admin:/home/Bill/session.json ./session.json
![num3](https://user-images.githubusercontent.com/32963758/164159548-d29e905a-da0d-48e7-95ed-c225dcaf2afa.gif)
