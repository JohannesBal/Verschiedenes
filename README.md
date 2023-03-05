# Verschiedenes

Das Repository "Verschiedenes" dient einer Script-Sammlung für neu aufgesetzte Betriebssysteme.

Als Grundlage wird nur der curl-Befehl benötigt um etwaige Instataltionen nachzuziehen.  

Installationen sind unterteilt nach Betriebssystem und Distribution


Übergangsweise:

export POD_NAME=$(kubectl get pods --namespace default -l "app.kubernetes.io/name=kubeview,app.kubernetes.io/instance=my-kubeview" -o jsonpath="{.items[0].metadata.name}")

echo "Visit http://127.0.0.1:8000/ to use your application"

kubectl --namespace default port-forward $POD_NAME 8000:8000
