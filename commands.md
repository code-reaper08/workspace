create cluster --name my-rubric-cluster --region us-east-1 --nodegroup-name my-rubric-nodes --node-type t3.small --nodes 1 --nodes-min 1 --nodes-max 2

```txt
2024-12-20 13:40:41 [ℹ]  eksctl version 0.133.0
2024-12-20 13:40:41 [ℹ]  using region us-east-1
2024-12-20 13:40:41 [ℹ]  skipping us-east-1e from selection because it doesn't support the following instance type(s): t3.small
2024-12-20 13:40:41 [ℹ]  setting availability zones to [us-east-1c us-east-1a]
2024-12-20 13:40:41 [ℹ]  subnets for us-east-1c - public:192.168.0.0/19 private:192.168.64.0/19
2024-12-20 13:40:41 [ℹ]  subnets for us-east-1a - public:192.168.32.0/19 private:192.168.96.0/19
2024-12-20 13:40:41 [ℹ]  nodegroup "my-rubric-nodes" will use "" [AmazonLinux2/1.24]
2024-12-20 13:40:41 [ℹ]  using Kubernetes version 1.24
2024-12-20 13:40:41 [ℹ]  creating EKS cluster "my-rubric-cluster" in "us-east-1" region with managed nodes
2024-12-20 13:40:41 [ℹ]  will create 2 separate CloudFormation stacks for cluster itself and the initial managed nodegroup
2024-12-20 13:40:41 [ℹ]  if you encounter any issues, check CloudFormation console or try 'eksctl utils describe-stacks --region=us-east-1 --cluster=my-rubric-cluster'
2024-12-20 13:40:41 [ℹ]  Kubernetes API endpoint access will use default of {publicAccess=true, privateAccess=false} for cluster "my-rubric-cluster" in "us-east-1"
2024-12-20 13:40:41 [ℹ]  CloudWatch logging will not be enabled for cluster "my-rubric-cluster" in "us-east-1"
2024-12-20 13:40:41 [ℹ]  you can enable it with 'eksctl utils update-cluster-logging --enable-types={SPECIFY-YOUR-LOG-TYPES-HERE (e.g. all)} --region=us-east-1 --cluster=my-rubric-cluster'
2024-12-20 13:40:41 [ℹ]  
2 sequential tasks: { create cluster control plane "my-rubric-cluster", 
    2 sequential sub-tasks: { 
        wait for control plane to become ready,
        create managed nodegroup "my-rubric-nodes",
    } 
}
2024-12-20 13:40:41 [ℹ]  building cluster stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:40:42 [ℹ]  deploying stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:41:12 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:41:42 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:42:42 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:43:42 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:44:42 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:45:43 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:46:43 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:47:43 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:48:43 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:49:43 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:50:44 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-cluster"
2024-12-20 13:52:46 [ℹ]  building managed nodegroup stack "eksctl-my-rubric-cluster-nodegroup-my-rubric-nodes"
2024-12-20 13:52:46 [ℹ]  deploying stack "eksctl-my-rubric-cluster-nodegroup-my-rubric-nodes"
2024-12-20 13:52:46 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-nodegroup-my-rubric-nodes"
2024-12-20 13:53:16 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-nodegroup-my-rubric-nodes"
2024-12-20 13:54:03 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-nodegroup-my-rubric-nodes"
2024-12-20 13:54:34 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-nodegroup-my-rubric-nodes"
2024-12-20 13:55:38 [ℹ]  waiting for CloudFormation stack "eksctl-my-rubric-cluster-nodegroup-my-rubric-nodes"
2024-12-20 13:55:38 [ℹ]  waiting for the control plane to become ready
2024-12-20 13:55:39 [✔]  saved kubeconfig as "/root/.kube/config"
2024-12-20 13:55:39 [ℹ]  no tasks
2024-12-20 13:55:39 [✔]  all EKS cluster resources for "my-rubric-cluster" have been created
2024-12-20 13:55:39 [ℹ]  nodegroup "my-rubric-nodes" has 1 node(s)
2024-12-20 13:55:39 [ℹ]  node "ip-192-168-54-143.ec2.internal" is ready
2024-12-20 13:55:39 [ℹ]  waiting for at least 1 node(s) to become ready in "my-rubric-nodes"
2024-12-20 13:55:39 [ℹ]  nodegroup "my-rubric-nodes" has 1 node(s)
2024-12-20 13:55:39 [ℹ]  node "ip-192-168-54-143.ec2.internal" is ready
2024-12-20 13:55:45 [ℹ]  kubectl command should work with "/root/.kube/config", try 'kubectl get nodes'
2024-12-20 13:55:45 [✔]  EKS cluster "my-rubric-cluster" in "us-east-1" region is ready
```
------

aws eks --region us-east-1 update-kubeconfig --name my-rubric-cluster

output: Added new context arn:aws:eks:us-east-1:667257161327:cluster/my-rubric-cluster to /root/.kube/config

-----

kubectl config current-context

output: arn:aws:eks:us-east-1:667257161327:cluster/my-rubric-cluster

-----

 kubectl get namespace

 output:
 NAME              STATUS   AGE
default           Active   36m
kube-node-lease   Active   36m
kube-public       Active   36m
kube-system       Active   36m

-----

    Database name: mydatabase
    User name: myuser
    Password: mypassword

-----

kubectl apply -f pvc.yaml
kubectl apply -f pv.yaml
kubectl apply -f postgresql-deployment.yaml

-----

kubectl get pods

postgresql-688c5c767c-r6947

-----

kubectl exec -it postgresql-688c5c767c-r6947 -- bash

----

kubectl apply -f postgresql-service.yaml

-----

kubectl get svc

-----

apt update
apt install postgresql postgresql-contrib

------

kubectl port-forward service/postgresql-service 5433:5432 &

--------

export DB_PASSWORD=mypassword
PGPASSWORD="$DB_PASSWORD" psql --host 127.0.0.1 -U myuser -d mydatabase -p 5433 < 1_create_tables.sql

export DB_PASSWORD=mypassword
PGPASSWORD="$DB_PASSWORD" psql --host 127.0.0.1 -U myuser -d mydatabase -p 5433 < 2_seed_users.sql

export DB_PASSWORD=mypassword
PGPASSWORD="$DB_PASSWORD" psql --host 127.0.0.1 -U myuser -d mydatabase -p 5433 < 3_seed_tokens.sql

-----

PGPASSWORD="$DB_PASSWORD" psql --host 127.0.0.1 -U myuser -d mydatabase -p 5433

-----

select * from users;

-----

exit and \q for quiting

----

# Update the local package index with the latest packages from the repositories
apt update

# Install a couple of packages to successfully install postgresql server locally
apt install build-essential libpq-dev

# Update python modules to successfully build the required modules
pip install --upgrade pip setuptools wheel

-----

pip install -r requirements.txt

-----

export DB_USERNAME=myuser
export DB_PASSWORD=${POSTGRES_PASSWORD}
export DB_HOST=127.0.0.1
export DB_PORT=5433
export DB_NAME=mydatabase

-----

python app.py

-----

add Werkzeug==2.2.2 in requirements.txt to solve ImportError: cannot import name 'url_quote' from 'werkzeug.urls' (/usr/local/lib/python3.8/dist-packages/werkzeug/urls.py)

----

curl <BASE_URL>/api/reports/daily_usage

in our context: curl 127.0.0.1:5153/api/reports/daily_usage

----

TypeError: Object of type function is not JSON serializable

This happens because we just name the function inside jsonify, which woudn't invoke the function,

```py

@app.route("/api/reports/daily_usage", methods=["GET"])
def daily_visits():
    # note here get_daily_visits() not get_daily_visits
    return jsonify(get_daily_visits())

```

----

curl 127.0.0.1:5153/api/reports/user_visits

----

apt update
apt install docker-ce docker-ce-cli containerd.io

-----

docker build -t test-coworking-analytics .

-----

docker run --network="host" test-coworking-analytics