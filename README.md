# hans

## Directory structure
- app/
  - entities/
  - usecases/
  - tests/
  
- delivery/
  - web_api/
  - nancy/
  - cli/
  - desktop/

- external/

## Commands
### Create new project
#### `hans new <project-name>`
Scaffolds empty project including `.travis.yml`, `.coveralls.yml`

#### `hans new usecase <usecase-name>`
Creates:
- `app/usecases/<usecase-name>.cs`
- `app/tests/usecases/<usecase-name>Tests.cs`
