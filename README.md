# HQLgen
Dataset for HQLgen.

## Description of each field
- **cleanedHql**: Rewritten HQL query according to the template (not used by HQLgen)
- **splitHql**: HQL query split by clause
   - **select**: **SELECT** clause
      - **agg**: Aggregate function if exists
      - **column**: Selected property (may be the whole class)
      - **fullExpr**: Full **SELECT** expression
   - **from**: Target class name
   - **where**: **WHERE** clause
      - **column**: Property of a condition
      - **op**: Operator of a condition
      - **value**: Placeholder, not predicted
      - **fullExpr**: Full **WHERE** expression
- **HQLMethod**: Target method name
- **HQLMethodParName**: Parameter names of the target method
- **HQLMethodParType**: Parameter types of the target method
- **HQLMethodComment**: Comment of the target method if exists
- **calledInMethod**: Method names of the methods that call the target method (call context)
- **calledInPar**: Parameter names in the call context
- **calledInParType**: Parameter types in the call context
- **column**: Candidate property names in the target class
- **columnType**: Types of the candidate properties
- **testFile**: Test project or not
- **projectName**: Project name
