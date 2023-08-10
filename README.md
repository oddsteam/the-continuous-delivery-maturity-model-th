# แปล The Continuous Delivery Maturity Model

|                        | Initial                                                                                                                                                            | Managed                                                                                                                                                                                       | Defined                                                                                                                                                                                                                                            | Quantitatively Managed                                                                                                                                            | Optimizing                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------- |
| Culture & Organization | - Teams organized based on platform/ technology<br/>- Defined and documented processes                                                                             | - One backlog per team <br/>- Adopt agile methodologies <br/>- Remove team boundaries                                                                                                         | - Extended team collaboration <br/>- Remove boundary dev/ ops<br/>- Common process for all changes                                                                                                                                                 | - Cross-team continuous improvement <br/>-Teams responsible all the way to production                                                                             | - Cross functional teams            |
| Build & Deploy         | - Centralized version control <br/>- Automated build scripts<br/>- No management of artifacts <br/>- Manual deployment<br/>- Environments are manually provisioned | - Polling CI builds<br/>- Any build can be re-created from source control<br/>- Management of build artifacts<br/>- Automated deployment scripts<br/>- Automated provisioning of environments | - Commit hook Cl builds<br/>- Build fails if quality is not met (code analysis, performance, etc.) <br/>- Push button deployment and release of any releasable artifact to any environment <br/>- Standard deployment process for all environments | - Team priorities keeping codebase deployable over doing new work <br/>- Builds are not left broken <br/>- Orchestrated deployments <br/>- Blue Green Deployments | - Zero touch Continuous Deployments |
| Release                | - Infrequent and unreliable releases <br/>- Manual process                                                                                                         | - Painful infrequent but reliable releases                                                                                                                                                    | - Infrequent but fully automated and reliable releases in any environment                                                                                                                                                                          | - Frequent fully automated releases <br/>- Deployment disconnected from release <br/>- Canary releases                                                            | - No rollbacks, always roll forward |
| Data Management        | - Data migrations are performed manually, no scripts                                                                                                               | - Data migrations using versioned scripts, performed manually                                                                                                                                 | - Automated and versioned changes to datastores                                                                                                                                                                                                    | - Changes to datastores automatically performed as part of the deployment process                                                                                 | - Automatic datastore               |

changes and rollbacks tested with every deployment
Test & Verification
• Automated unit tests Separate test environment
• Automatic Integration Tests
• Static code
analysis • Test coverage analysis
Automatic functional tests
Manual performance/ security tests
Fully automatic acceptance tests
• Automatic performance/security tests
Manual exploratory testing based on risk based testing analysis
Verify expected business value
• Defects found and fixed immediately (roll forward)
Information & Reporting
Baseline process metrics • Manual reporting Visible to report runner
• Automatic generation of release notes
Measure the
process • Automatic reporting • Visible to team
Pipeline traceability Reporting history
• Visible to cross-silo
Dynamic self-service of information
Report trend analysis
• Real time graphs on deployment pipeline metrics
Customizable dashboards • Cross-reference across
organizational boundaries

อ้างอิงจาก [The Continuous Delivery Maturity Model](https://tech.aabouzaid.com/2016/01/continuous-delivery-and-maturity-model.html)
