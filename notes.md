# DEXL syntax

**experiment** load-congestion-levels {
  model: ANOVA,
  factors: 1,
  depdendent: {
      name: latency
      collector: dome_challenge_x2
  },
  independent:[
    {name: load, collector: "pdx-load"},
    {name: tm-action, collector: "tm-actions"}
  ],
  notebook: load-congestion-levels_analysis
}


**collector** pdx-load {
    image: pdk-load data
    secrets: secretsfile
}

**collector** scamper {
    image: cloudflare/scamper
    secrets: secretfile
}

**notebook** labnotes {
  secrets: secretfile
}


DOME.validate_experiment()
DOME.register_experiment()
DOME.register_collector()
DOME.customer_collector()
DOME.generate_challenge(
  catalog: ANOVA-one-away
)


