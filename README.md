# Set Up a Virtual Python Environment & installing-theHarvester at the same time

<h3> This virtual enviornment is necessary when you are using virtual machine or Usually when you'll get an error  ---></h3> <h2>"externally-managed-environment" </h2> <h3>which means your python environment that is managed outside of the package manager or virtual environment tool. 
. </h3>

Then use this commands serially ------->

1. apt install python3-virtualenv  --> #Install the virtual Environment

2. virtualenv /venv  --->  # Create a virtual environment

3. source venv/bin/activate  <h3>OR</h3> source /venv/bin/activate (if you do from other directory) --> # Activate the virtual environment

4. git clone https://github.com/laramies/theHarvester  ------> #Clone the directory to your linux pc.

5. cd theHarvester ----> #Go to theHarvester directory.

6. sudo apt install python3-pip  ------> #To install pip.

7. pip3 install -r requirements.txt ----> need to install the requirement everytime after creating virtual enviornment.

python3 theHarvester.py -d example.com -b all ---> #Here all means all search engines.

when done you can deactivate the environment using the command ----> <h3>deactivate</h3>

<h2>To reactivate the virtual Environment Again/Later</h2>

<h3>Navigate to the directory where your virtual environment is located. then type the 3rd command</h3>

<h3>If you want to create another enviornment in another directory then type 2nd and 3rd command</h3>

<h2> How to add API Keys in Harvester for more accurate results</h2>
Some private search engines like shodan, virusdefender etc needs to add their API in the harvester for searching. to add their API just login to those websites and copy their respective APIs. Then edit this file
<h4>sudo mousepad /etc/theHarvester/api-keys.yaml</h4>
from there add the API keys under there names according to serial. then save it. 
then when you'll search again something, system will search from those websites also using the APIs.
