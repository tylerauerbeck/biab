FROM quay.io/ansible-tower/ansible-tower

USER root

RUN sh -c ". /var/lib/awx/venv/ansible/bin/activate ; pip install boto==2.49.0 boto3==1.9.200 awscli==1.16.210 ansible-tower-cli==3.3.6"

ENTRYPOINT ["tini", "--"]

CMD /usr/bin/launch_awx.sh

