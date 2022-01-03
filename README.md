Follow these steps:

1. Install python-pip on ansible master as a root user
    # sudo apt-get update
    # sudo apt-get install python-pip

2. Install boto using pip
    # pip install boto

3. Create an aws IAM admin user

4. Provide IAM user details on the .boto file
    # vi .boto
    # change to insert mode
    [Credentials]
    aws_access_key_id=XXXXX
    aws_secret_access_key=XXXX

5. Create an ec2 AMI 

6. Change to ansible user
    # su username

7. Clone this repo 

8. Change the group variable in myec2nodes file under group_vars

9. Run the playbook
    $ ansible_palybook -i myhosts ec2nodesplaybook.yml

10. To Check and verify aws ec2 instance creation

11. Dont forget to terminate the ec2 instances!!

