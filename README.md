# AOG-Job-manager
Job manager for AgOpenGPS in Node-Red

![image](https://github.com/bitfieldfarm/AOG-Job-manager/assets/98184919/944b3963-29af-4c1e-9b73-d698fd556425)

It creates an activity log in farmOS based on the filename used for the field in AgOpenGPS.
The filename sould be in this format "Field Vehicle Date"
And the field name have to match with field asset name in farmOS.

Working dir has to be set. Should be the path to where AgOpenGPS store the fields. (The folder you have to open to view the fields dirs)

Then it should get the most recent field worked on, and save the log in farmOS.
Flags, boundary and section covarage are imported to map in log.
Also, worked area are stored in note-field.

### Setup
Must have a working instance of [farmOS](https://farmos.org). Selfhosted or hosted at [Farmier](https://farmier.com)
Also Node-Red running on the tablet running AgOpenGPS

And some extra libraries for node-red..
npm install togeojson wellknown 
npm install xmldom

I also used the farmOS API nodes from Farmer Ed.
Install instructions here [Farmer-Eds-Shed](https://github.com/Farmer-Eds-Shed/Node-Red-4-farmOS)
 

I'm surprised if there are no bugs.

Use at own risk

![image](https://github.com/bitfieldfarm/AOG-Job-manager/assets/98184919/e8c3c36a-9044-4c68-9677-5cc729b827f5)
