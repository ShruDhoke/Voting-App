<h1>Run the app in Kubernetes</h1>
The folder k8s-specifications contains the YAML specifications of the Voting App's services.

Run the following command to create the deployments and services. Note it will create these resources in your current namespace (default if you haven't changed it.)

kubectl create -f Voting-app/

The vote web app is then available on port 31000 on each host of the cluster, the result web app is available on port 31001.

To remove them, run:

kubectl delete -f  Voting-app/

<h1 align="center">Architecture</h1>
<img align="right" alt="Coding" width="400" src="https://miro.medium.com/v2/resize:fit:1400/format:webp/0*alcCLL8fj9_fZycq.png">

A front-end web app in <a href="https://www.python.org/">Python</a> which lets you vote between two options

A <a href="https://redis.io/">Redis</a> which collects new votes

A <a href="https://en.wikipedia.org/wiki/.NET_Framework">.NET</a> worker which consumes votes and stores them in…

A <a href="https://www.postgresql.org/">Postgres</a> database backed by a Docker volume

A <a href="https://nodejs.org/en">Node.js</a> web app that shows the results of the voting in real time

<h1 align="center">Output</h1>
<img align="right" alt="Coding" width="400" src="https://miro.medium.com/v2/resize:fit:828/format:webp/0*1hEHz5Nj9V7_rGCR.png">


