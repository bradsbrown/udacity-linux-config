## Linux Server Setup

# Server Information:
- IP: 52.41.175.230
- Port: 2200

# Web URL
- http://ec2-52-41-175-230.us-west-2.compute.amazonaws.com/

# Third Party Resources
- For a few sticky issues, I searched for help from StackOverflow
- For most of the setup, the guide linked in the project details notes, [Markedly underwhelming and potentially wrong...](https://discussions.udacity.com/t/markedly-underwhelming-and-potentially-wrong-resource-list-for-p5/8587), did the trick for me.

# Summary of Changes Made
- Installed:
  - updated apt-get list and upgraded installed packages
  - psychopg2
  - flask
  - apache
  - mod_wsgi
  - virtualenv
  - sqlalchemy
  - git
  - cloned in my catalog project
- Edited:
  - time zone to UTC
  - added user 'grader'
  - gave 'grader' sudo privileges
  - set ufw to default deny incoming requests, save ports 2200, 80, and 123
  - verified PSQL only accepts connections from local/127.0.0.1
  - added appropriate wsgi hooks and apache .conf files to link to project
