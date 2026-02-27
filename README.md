# controller-credential_types-global

Shared credential type definitions

## CasC Key

```
controller_credential_types
```

## Usage

Place JSON files in this repository using the `controller_credential_types` key.
The CasC dispatcher will automatically pick up and apply these configurations
to AAP when the CI/CD pipeline triggers.

### Example

```json
{
    "controller_credential_types": [
        {
            "name": "example-resource",
            "description": "Replace with your actual configuration"
        }
    ]
}
```

## CI/CD Pipeline

This repository includes a thin CI/CD caller that triggers the platform's
shared CasC pipeline on push and pull request events. The pipeline validates
JSON files and triggers the dispatcher Job Template in AAP.

## Part of the Hybrid CasC Solution

This repository is managed by the **aap-casc-platform-demo** platform team as part
of the Hybrid AAP Configuration-as-Code framework. See the
[aap-casc-engine](../aap-casc-engine) repository
for full documentation.
