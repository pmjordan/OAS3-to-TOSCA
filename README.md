# OAS3-to-TOSCA

The repo records the result of an experimental mapping of a sample OAS3 file [Pet Store](Pet.json), into a TOSCA interface type defintion [TOSCA_API_interface.yml](TOSCA_API_interface.yml). Only a one or two examples of each structure type found in the source were mapped. The mapping was mostly manual but an online tool was used to convert YAML to JSON, there is a folder of [intermediate results](intermediate-steps).

The TOSCA Interface type was then used in a node type defintion [line 201 in](TOSCA_API_interface.yml) and that node type used in a topology template [line 252 in](TOSCA_API_interface.yml).

The TOSCA Interface type was also used in a relationship type defintion and that relationship type used between two nodes in a toplology template, all in [TOSCA_API_relationship.yml](TOSCA_API_relationship.yml)

Notifications using callbacks were a particular problem to map and were recorded in [TOSCA_API_notification.yml](TOSCA_API_notification.yml)

My conclusion was that it would be possible to write an automatic translator which took and OAS3 spec and an input and created TOSCA interface type defintion as an output.
