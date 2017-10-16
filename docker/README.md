ZooKeeper Container for OpenShift 3
===================================

Version of a popular ZooKeeper Docker image (docker pull spec: confluentinc/cp-zookeeper)
that will run on OpenShift 3 with the default Security Context Constraint (SCC)
of restricted.

The cp-zookeeper docker image (at least version 3.3.0) runs fine under the **restricted** SCC already,
so no customization of the image is required at this time.

# Importing Docker image into OpenShift
There is a YAML file in the openshift directory (zookeeper-imagestream.yml) which will
import the confluentinc/cp-zookeeper image(s) into the internal registry of an OpenShift
cluster.
