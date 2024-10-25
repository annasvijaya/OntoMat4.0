# Ontomat4.0: Ontology for I4.0 Maturity Model

OntoMat 4.0 is a conceptual framework developed to assess the maturity of organizations in their Industry 4.0 (I4.0) digital transformation journeys. It leverages a series of structured classes and object properties that reflect both technical and non-technical aspects of digital readiness and organizational growth. This project is informed by research and reference architecture models, providing companies with a clear path to evaluate and enhance their digital transformation processes.

## Overview of Core Classes

The core classes in OntoMat 4.0 model the key aspects of Industry 4.0 maturity, capturing factors influencing success, the maturity of dimensions, and the causal relationships between various drivers.

### 1. Factor
- **Description**: Represents critical driving forces in an organization’s I4.0 maturity, covering both technical and non-technical elements such as IT infrastructure or organizational culture.
- **Key influencing drivers used to evaluate I4.0 maturity.**
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
- **Object Properties**:
  - `hasObjective`: Links each factor to its goals (e.g., Advanced IT to real-time data analytics).
  - `hasDimension`: Associates each factor with a Dimension.
  - `hasWeight`: Indicates the relative importance of each factor, helping prioritize areas in digital transformation.

### 2. Dimension
- **Description**: Provides a structured grouping of factors representing essential categories (e.g., Technology, Culture, Governance) critical for assessing I4.0 maturity.
- **Represents critical areas or dimensions within the I4.0 maturity model.**
  - Culture
  - OrganizationGovernance
  - Process_Operation
  - Product
  - Resource
  - Technology
- **Object Properties**:
  - `hasDimension`: Connects factors with overarching themes, facilitating a comprehensive maturity assessment.

### 3. MaturityLevel
- **Description**: Identifies the organization’s overall stage in digital maturity, from initial adoption to complete digital integration.

### 4. DimensionMaturity
- **Description**: Evaluates the combined maturity of factors within a Dimension, highlighting specific areas needing development.
  - **Example**: If Technology includes Advanced IT and Data and Information, DimensionMaturity reflects the aggregate maturity of these factors.

### 5. FactorMaturity
- **Description**: Measures the maturity of individual factors, helping organizations identify areas contributing to their overall maturity.
- **Sub-properties**:
  - `CurrentFactorMaturity`: The current state of maturity.
  - `TargetFactorMaturity`: Desired future state of maturity.
- **Object Properties**:
  - `meetsIndicator`: Links maturity with indicators validating each factor’s progress.
  - `hasCurrentFM` and `hasTargetFM`: Track current and target maturity for each factor.

### 6. AssessmentNode
- **Description**: Represents assessment points linking FactorMaturity to criteria, producing scores that help determine MaturityLevel, DimensionMaturity, and FactorMaturity.

### 7. AssessmentScore
- **Description**: Numerical score assigned to each factor during maturity assessment, indicating progress toward I4.0 goals.
- **Object Properties**:
  - `hasScore`: Stores maturity scores.
  - `determineML`, `determineDM`, `determineFM`: Links scores to maturity levels, dimensions, and factors respectively.

### 8. Objective
- **Description**: Defines specific goals that organizations aim to achieve for maturity.
- **Object Properties**:
  - `hasIndicator`: Connects objectives with measurable indicators of success.

### 9. Indicator
- **Description**: Measurable criteria used to assess if objectives are met, tracking the effectiveness of factors.
- **Object Properties**:
  - `IsScoreOfIndicator`: Connects AssessmentScore to indicators defining success for each factor.

### 10. Company
- **Description**: Represents the entity undergoing the I4.0 evaluation.
- **Object Properties**:
  - `hasFM`, `hasML`, `hasDM`: Track Factor, Maturity, and Dimension Maturity, respectively, for the organization.

### 11. Weight
- **Description**: Defines the relative importance of various factors, aiding prioritization during digital transformation.
- **Object Properties**:
  - `hasCriteria`: Links Weight to criteria used to evaluate its significance.

### 12. CausalRelationship
- **Description**: Models cause-and-effect between factors, providing insights into interdependencies and guiding strategic decisions.
- **Object Properties**:
  - `hasCause` and `hasEffect`: Model the influence of one factor over another (e.g., how Data and Information improvements enhance Asset Utilization).

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

