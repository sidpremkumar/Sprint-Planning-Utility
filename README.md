<h1 align="center"> Sprint Planning Service :pear:</h1>
<a href='https://sprint-planning-utility.readthedocs.io/en/latest/?badge=latest'>
    <img src='https://readthedocs.org/projects/sprint-planning-utility/badge/?version=latest' alt='Documentation Status' />
</a>

### Config 
The [config](SPU/config.py) file is used to: 
1. Set the `operational_q1_start`
1. Set the `default_jira_instance` and other JIRA credentials 
1. Teams and relevant information
1. Finally add the following environmental variables: 

    `GLOBAL_BOARD :: Name of the global JIRA board`
    
    `GLOBAL_BAD_BOARD : Name of the global bad JIRA board`

Optionally the `run_for_quarter` field can be set to run the utility for a specific quarter
 

### Running 
You can run the program by installing it first: 

    > python setup.py install

Set up the [config](SPU/config.py) file.

Then run the program by typing:

    > spu
    
### Troubleshooting

If you get a SSL: CERTIFICATE_VERIFY_FAILED error. Please try to run this in your terminal: 

    > export REQUESTS_CA_BUNDLE=/etc/pki/tls/certs/ca-bundle.trust.crt