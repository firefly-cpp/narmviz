# narmviz

narmviz provides visualization tools for numerical association rules derived from transactional datasets. It supports numerical and categorical
attribute visualization and time-series data representation for rule-based insights.

## 📦 Installation

```
TODO
```

## 🚀 Usage

### Basic run example

```R
library(narmviz)

dataset <- read.csv("random_sportydatagen.csv")

# Define antecedents
antecedent <- list(
  list(name = "duration", min = 50, max = 65),
  list(name = "distance", min = 15.0, max = 40.0)
)

# Define consequents
consequent <- list(
  list(name = "calories", min = 200.0, max = 450.0),
  list(name = "descent", min = 50.0, max = 140.0)
)

# Define rule
rule <- list(antecedent = antecedent, consequent = consequent)

# Visualize rule
visualize(rule, dataset, path = "example.pdf", allfeatures = TRUE, antecedent = TRUE, consequent = TRUE, timeseries = TRUE, intervalcolumn = "interval", interval = 3)
```

## 📚 References

Ideas are based on the following research papers:

[1] Fister Jr, I., Fister, I., Fister, D., Podgorelec, V., & Salcedo-Sanz, S. (2023). [A comprehensive review of visualization methods for association rule mining: Taxonomy, Challenges, Open problems and Future ideas](https://arxiv.org/abs/2302.12594). arXiv preprint arXiv:2302.12594.

[2] Fister Jr, I., Fister, D., Fister, I., Podgorelec, V., & Salcedo-Sanz, S. (2022). [Time series numerical association rule mining variants in smart agriculture](https://arxiv.org/abs/2212.03669). arXiv preprint arXiv:2212.03669.

[3] I. Fister Jr., I. Fister [A brief overview of swarm intelligence-based algorithms for numerical association rule mining](https://arxiv.org/abs/2010.15524). arXiv preprint arXiv:2010.15524 (2020).

[4] I. Fister Jr., A. Iglesias, A. Gálvez, J. Del Ser, E. Osaba, I Fister. [Differential evolution for association rule mining using categorical and numerical attributes](http://www.iztok-jr-fister.eu/static/publications/231.pdf) In: Intelligent data engineering and automated learning - IDEAL 2018, pp. 79-88, 2018.

## 🔗 Related software

[NiaARM.jl](https://github.com/firefly-cpp/NiaARM.jl)

## 📄 Cite us

Fister, I. Jr, Fister, I., Podgorelec, V., Salcedo-Sanz, S., & Holzinger, A. (2024). NarmViz: A novel method for visualization of time series numerical association rules for smart agriculture. Expert Systems, 41(3), e13503. [https://doi.org/10.1111/exsy.13503](https://doi.org/10.1111/exsy.13503)

## 🔑 License

This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.

## Disclaimer

This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
