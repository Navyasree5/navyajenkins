# company-landingpage
Deploy the changes in company-landingpage to google cloud
## installetion of gcloud
      Before you begin
           1.Create a Google Cloud Platform project, if you don't have one already.
           2.Download the Google Cloud SDK installer.(https://dl.google.com/dl/cloudsdk/channels/rapid/GoogleCloudSDKInstaller.exe)
All of the installation methods above install the default Cloud SDK components, which include gcloud, gsutil and bq command-line tools.
## Initialize the Google Cloud SDK
           1.Run the following at a command prompt:
                                    # gcloud init.
           2.log in using your Google user account & select a Cloud Platform project.
           3.select default Compute Engine zone.
## rsync is a utility for efficiently transferring and synchronizing files between a computer and an external hard drive and across networked computers by comparing the modification times and sizes of files.
To sync the contents of the local directory "data" to the bucket gs://mybucket
Command:
       # gsutil rsync data gs://mybucket
To recurse into directories use the -r option
Command:
       # gsutil rsync -r data gs://mybucket/data      
