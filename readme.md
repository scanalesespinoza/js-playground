JS Playground
=============
Collection of my Javascript experiments, mostly published on codepen.io. Feel free to use the source code as you wish.

Demos:
=============
* Canvas Asteroids: http://codepen.io/everblind/details/bzBsp

Openshift Lab:
==============
```
oc login https://cloud.cnad.io:443 --token=<TOKEN>
oc project <MI-PROYECTO>
oc delete service,pod,deploymentconfig,buildconfig,build,imagestream --all -n taller-devops
oc new-app openshift/httpd:latest~https://github.com/scanalesespinoza/js-playground.git --context-dir=canvas-asteroids
oc status
oc get build
oc get buildconfig
oc get deploymentconfig
oc get pods
oc get service
oc get route
oc expose service js-playground
oc get route
oc delete service,pod,deploymentconfig,buildconfig,build,imagestream --all -n <MI-PROYECTO>
```

License
=============
Copyright (c) Jeff Ibacache. See the LICENSE file for license rights and limitations (MIT).
