<h1>Run the app in Kubernetes</h1>
The folder named Voting-app contains the YAML specifications that are required to deploy the Voting App's services. To create the deployments and services, you can run the following command. It is important to note that this command will create these resources in your current namespace (default if you haven't changed it).

<br>kubectl create -f Voting-app/

If you wish to remove these resources, you can run the following command:

kubectl delete -f Voting-app/

<h1 align="center">Architecture</h1>
<img align="right" alt="Coding" width="400" src="https://miro.medium.com/v2/resize:fit:1400/format:webp/0*alcCLL8fj9_fZycq.png">

A front-end web app in <a href="https://www.python.org/">Python</a> which lets you vote between two options

A <a href="https://redis.io/">Redis</a> which collects new votes

A <a href="https://en.wikipedia.org/wiki/.NET_Framework">.NET</a> worker which consumes votes and stores them in…

A <a href="https://www.postgresql.org/">Postgres</a> database backed by a Docker volume

A <a href="https://nodejs.org/en">Node.js</a> web app that shows the results of the voting in real time

<h1 align="center">Output</h1>
<img align="right" alt="Coding" width="400" src="https://miro.medium.com/v2/resize:fit:828/format:webp/0*1hEHz5Nj9V7_rGCR.png">


