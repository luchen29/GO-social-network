# GO-social-network-application

This is a social network application for users to post media including pictures and short videos. 
Backend-server implemented based on Go language.

The project was built on Google Cloud Platform; 
Images and all media files are stored in Google Cloud Storage;
Cloud-based ML is implemented on Google Cloud AI Platform.

Key Features:
* Use Elastic Search for complex data searching.
* Storing data to GCP BigTable (in case large data traffic).
* Use Dataflow for data transmition and Big Query for offline data analysis.
* Buid up a ML Model in recognizing human face among all media pictures.
