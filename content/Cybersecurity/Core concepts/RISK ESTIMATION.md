Risk estimation is a critical aspect of cybersecurity, aimed at identifying and assessing potential threats and vulnerabilities in order to prioritize and mitigate risks effectively.
#### Key Terms:

- **Asset**: The set of goods, data, and people needed for an IT service. Assets can be hardware, software, data, or human resources.
- **Vulnerability**: An intrinsic weakness of an asset. For example, a password used for login could be vulnerable to brute-force attacks, or a server might be susceptible to flooding.
- **Threat**: A possible deliberate action or accidental event that can exploit a vulnerability, leading to the loss of a security property (e.g., confidentiality, integrity, availability). Threats depend on the specific environment or operational conditions.
- **Attack**: The actual occurrence of a threat due to a deliberate action, such as a hacking attempt.
- **(Negative) Event**: The occurrence of a threat due to an accidental event, like a hardware failure.
#### The Risk Estimation Matrix:

A **Risk Matrix** is used to assess the level of risk by combining the **impact** of an event and its **probability** of occurrence. This helps prioritize risks based on their potential severity and likelihood.

|                        | **Frequent (5)** | **Probable (4)** | **Occasional (3)** | **Remote (2)** | **Improbable (1)** |
|------------------------|------------------|------------------|--------------------|----------------|--------------------|
| **Catastrophic (5)**    | 25               | 20               | 15                 | 10             | 5                  |
| **Significant (4)**     | 20               | 16               | 12                 | 8              | 4                  |
| **Moderate (3)**        | 15               | 12               | 9                  | 6              | 3                  |
| **Low (2)**             | 10               | 8                | 6                  | 4              | 2                  |
| **Negligible (1)**      | 5                | 4                | 3                  | 2              | 1                  |

- **Impact**:
    
    - Catastrophic (5): Severe financial losses, critical system disruptions.
    - Significant (4): Major disruptions, but systems recoverable with significant effort.
    - Moderate (3): Noticeable disruptions with manageable recovery costs.
    - Low (2): Minor issues with limited consequences.
    - Negligible (1): Insignificant effects on operations or business.
- **Probability**:
    
    - Frequent (5): The event is highly likely to occur in the near term.
    - Probable (4): The event is likely to occur over time.
    - Occasional (3): The event could occur, but not frequently.
    - Remote (2): The event is unlikely to occur.
    - Improbable (1): The event is highly unlikely to happen.

The Risk Estimation Matrix gives an useful visualization tool to explain the most important security measure to take in that moment based on frequency and potential disruption of the threat.
In fact in a business or in an organization you don't have an infinite amount of resources(human and financially), so more often than not you have to decide on which aspects you want to improve on. (The example could be everything over 15 on the risk Estimation Matrix)
