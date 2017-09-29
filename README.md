# hans

## Directory structure
- app/
  - entities/
  - usecases/
  - tests/
    - entities/
    - usecases/
  
- delivery/
  - api/
  - cli/
  - desktop/

- external/
  - database/
  - filesystem/
  - logging/
  - rest/

## Commands
### Create new project
#### `hans new <project-name>`
Scaffolds empty project including `.travis.yml`, `.coveralls.yml`

#### `hans new usecase <usecase-name>`
Creates:
- `app/usecases/<usecase-name>/<usecase-name>UseCase.cs` (Implements IUseCase)
- `app/usecases/<usecase-name>/<usecase-name>InputBoundary.cs` (IUseCase { void Execute(); })
- `app/usecases/<usecase-name>/<usecase-name>OutputBoundary.cs` (IPresenter { ViewModel GetViewModel(); })
- `app/usecases/<usecase-name>/<usecase-name>Presenter.cs` (Implements IPresenter)
- `app/tests/usecases/<usecase-name>/<usecase-name>UseCaseTests.cs`


#### `hans new entity <entity-name>`
Creates:
- `app/entities/<entity-name>.cs`
- `app/tests/entities/<entity-name>Tests.cs`
