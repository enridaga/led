# led




Prepare the data from the led archive:

```bash
fx -q fx/listening-experiences.sparql -l archives/led-SNAPSHOT.nt -o database/listening-experiences.csv
```

Generate data graphs for each listening experience:

```bash
fx -q fx/generate-turtles.sparql -l archives/led-SNAPSHOT.nt -v database/listening-experiences.csv -p database/?id/graph.ttl
```

