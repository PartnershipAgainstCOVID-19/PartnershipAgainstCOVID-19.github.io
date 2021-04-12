# Partnership against COVID-19

## Who are we?
- robo4you - [https://robo4you.at/](https://robo4you.at/)
- CYBERTEC - Data Science & PostgreSQL - [https://www.cybertec-postgresql.com/](https://www.cybertec-postgresql.com/)
- spaceteam TU Wien - [https://spaceteam.at](https://spaceteam.at)

## How do we help fight COVID-19?

As COVID-19 is spreading in Austria we use freed up computer resources to help research in predicting protein structures. We use the [BOINC client](https://boinc.berkeley.edu/index.php) developed by the Berkley University and contribute to the [Rosetta@Home project](https://boinc.bakerlab.org/rosetta/).

### Results
"We are happy to report that the Rosetta molecular modeling suite was recently used to accurately predict the atomic-scale structure of an important coronavirus protein weeks before it could be measured in the lab. Knowledge gained from studying this viral protein is now being used to guide the design of novel vaccines and antiviral drugs."

Source: [https://www.ipd.uw.edu/2020/02/rosettas-role-in-fighting-coronavirus/](https://www.ipd.uw.edu/2020/02/rosettas-role-in-fighting-coronavirus/)

## How can I help?

The [BOINC client](https://boinc.berkeley.edu/index.php) works on every PC no matter how slow. Even android phones can contribute to the research.

### Installing BOINC

Download Link: [https://boinc.berkeley.edu/download.php](https://boinc.berkeley.edu/download.php)

After installing the Software, BOINC will ask you to add a project. Search for Rosetta@Home in the list then click "add". Create an account for the project and then your PC will start downloading new tasks.

#### Recommended settings:
You can configure your client in ```Options``` -> ```Computing Preferences```. <br>

### Join our team: [here](https://boinc.bakerlab.org/rosetta/team_display.php?teamid=19523)

#### How to join?
Login online to the Rosetta project [here](https://boinc.bakerlab.org/rosetta/home.php) then click on "Find Team" and search for "Partnership against COVID-19" or go directly to the team and click join: [on our team page](https://boinc.bakerlab.org/rosetta/team_display.php?teamid=19523)

### Installation on Linux
#### For Linux users an package exists for most distributions
For Debian and its derivatives run
```bash
sudo apt install boinc
```
and then launch the client and add the rosetta project over the gui.

#### Installing BOINC on a server

As most servers don't have a GUI the installation must be done over the command line. <br>

Example for an installation on a Debian or Ubuntu server:

```bash
sudo apt install boinc -y
```

After installing BOINC a new project can be added with the tool ```boinccmd```

If you don't want to create an account the next command is sufficient. This will credit your work to a user in our team and you won't have to register for Rosetta@Home.

```bash
boinccmd --project_attach http://boinc.bakerlab.org/rosetta/ 1884336_1e4743d230b29ad48247dc303d9b6c39
```

1. However, if you want your work to be credited to an account you will have to create one [here](https://boinc.bakerlab.org/rosetta/create_account_form.php)
1. Then go to the site "[get account keys](https://boinc.bakerlab.org/rosetta/weak_auth.php)" and copy your account key.
1. Then run this command and replace ```key``` with your copied one.

```bash
boinccmd --project_attach http://boinc.bakerlab.org/rosetta/ key
```

After creating your own account you can join [our team](https://boinc.bakerlab.org/rosetta/team_display.php?teamid=19523) and compare your earned points with other users.
