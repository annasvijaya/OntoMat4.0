# Ontomat4.0: Ontology for I4.0 Maturity Model

Ontomat4.0 is an ontology designed to represent the Industry 4.0 (I4.0) maturity model. It provides a structured framework for assessing the maturity level of organizations in their adoption and implementation of Industry 4.0 principles and technologies.

## Overview

The Ontomat4.0 ontology comprises classes and relationships that represent various aspects of the I4.0 maturity model, including dimensions, factors, indicators, and maturity levels.

## Classes

### Dimension
- Represents critical areas or dimensions within the I4.0 maturity model.
  - Culture
  - OrganizationGovernance
  - Process_Operation
  - Product
  - Resource
  - Technology

### Factor
- Description: Represents the critical driving forces in an organization’s Industry 4.0 maturity, covering both technical and non-technical elements such as IT infrastructure or organizational culture.
- Key influencing drivers used to evaluate I4.0 maturity.
  - AdvancedIT
  - Agility
  - AssetUtilization
  - Collaboration
  - DataAnalyticsInUsagePhase
  - DataAndInformation
  - DigitalLeadershipCapability
  - Employee
  - ICTAddOnFunctionalities
  - InnovationManagement
  - Integration
  - InventoryAndSupplyChain
  - InvestmentForI40
  - Quality
  - StrategyForI40
  - WillingnessToChange
- Object Properties:
  - hasObjective: Links each factor to its goals (e.g., Advanced IT to real-time data analytics).
  - hasDimension: Associates each factor with a Dimension.
  - hasWeight: Indicates the relative importance of each factor, helping prioritize areas in digital transformation.


### Indicator
- Specific measures used to assess the maturity level of factors.

### MaturityLevel
- Represents the overall maturity level of a company or specific dimensions and factors.

### Objective
- Specific goals set to achieve I4.0 maturity.

### Weight
- Represents the importance or influence of factors or indicators on overall maturity.

## Usage

This ontology can be used for:
- Assessing the maturity level of organizations in their Industry 4.0 journey.
- Developing maturity assessment tools and methodologies.
- Analyzing and comparing maturity levels across different dimensions and factors.

## License

This ontology is available under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

## Acknowledgments

This ontology is developed as part of PhD Project in I4.0 Maturity of  INDEED Research Group at Constructor University, Bremen, Germany.

## Contributors

- Linda Salma Angreani
- Annas Vijaya
- Hendro Wicaksono

