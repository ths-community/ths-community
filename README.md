# THS-Community

![](https://www.ths-greifswald.de/wp-content/uploads/2019/01/Design-Logo-THS-deutsch-271.png)

## About
The goal of this set of repositories is to collect tips, tricks and code examples for [E-PIX](https://ths-greifswald.de/e-pix), [gPAS](https://ths-greifswald.de/gpas) and [gICS](https://ths-greifswald.de/gics) from the community in one place and to promote the exchange of experiences among our users.
The initial idea for this GitHub exchange came from colleagues at Siemens Healthineers and LMU Munich. Many thanks :)
        
## Repositories   
Separate [Repositories](https://github.com/ths-community?tab=repositories) for individual topics and community-projects can easily be created after short consultation with us.

### Ongoing community-work for E-PIX, gPAS, gICS includes 
- Kubernetes-scripts for E-PIX, gPAS, gICS 
- Podman-scripts for gICS as an alternative for Docker
- NodeJs-based Webfrontend for E-PIX, gPAS, gICS 
- *[Redcap-Integration based on SOAP for E-PIX and gPAS (external repo)](https://github.com/cerhardt/redcap-pseudo-service)*

See the [list of repositories](https://github.com/ths-community?tab=repositories) for details and to get in contact with the respective collaborators.

### Use of SSH keys to push/commit to ths-community-project
Scenario: 
- use of multiple accounts on Github to push/commit into ths-community-projects
- all accounts have to ssh to Github as git@github.com
- the ssh key is used to determine which Github user you are
- in this case neither .ssh/config nor ssh-agent will work

Solution:

- Create a local repository:

`git clone -c core.sshCommand="/usr/bin/ssh -i /home/me/.ssh/id_rsa_foo" git@github.com:me/repo.git`

- Once you've cloned the repository you can use the git config command to set this permanently: 

`git config --local core.sshCommand "/usr/bin/ssh -i /home/me/.ssh/id_rsa_foo"`

References: [stackoverflow, accessed 2023-07-26](https://stackoverflow.com/questions/6688655/select-private-key-to-use-with-git#41947805)

## Additional Information

E-PIX, gPAS, gICS, TTP-Dispatcher, TTP-FHIR-Gateway and NotificationService (+Client) were developed and published from 2013 (til today) by the University Medicine Greifswald.

### License

License: AGPLv3, https://www.gnu.org/licenses/agpl-3.0.en.html

### Contact and Community Dialog
If you have any questions, please do not hesitate to contact us: [kontakt-ths@uni-greifswald.de](mailto:kontakt-ths@uni-greifswald.de) and take advantage of our regular [community dialog](https://ths-greifswald.de/community).
