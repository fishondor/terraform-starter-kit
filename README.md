## Steps

### Create a new project in GCP
* Go to https://console.cloud.google.com/
* Press project selector -> NEW PROJECT
* Create service account and generate key:
    * IAM & Admin -> Service Accounts
    * CREATE SERVICE ACCOUNT
    * Set account role to ```editor```
    * Press the new created service account and then KEYS
    * ADD KEY -> Create new key -> JSON
    * Key will be downloaded to your local computer. Copy it to our working directory or any other location you see fit

### Start a Terraform project
* Clone this repo
#### mac, linux
* Run ```terraformw``` - this will download terraform 1.0.8 to .bin folder in your current project
#### Windows
* Download executable file from https://www.terraform.io/downloads.html
* Extract the downloaded zip and place the exe file in your project folder
* https://learn.hashicorp.com/tutorials/terraform/install-cli?in=terraform/gcp-get-started

### Managing resources
* https://learn.hashicorp.com/tutorials/terraform/google-cloud-platform-build?in=terraform/gcp-get-started
* Rename or copy main.tf.example to main.tf
* Update service key path and project ID
* ```terraform -help```
* ```terraform init```
* ```terraform plan```
* ```terraform apply```
* ```terraform plan -destroy```
* ```terraform destroy```