# Architecture Overview

```mermaid
classDiagram
    hide empty members
    class MainController {
        %% empty %%
    }
    class ProfileListController
    class ProfileEditorController
    class SceneEditorController
    class Navigator
    class EventBus
    class Repository 
    class ProfileEditorView
    class ProfileListView
    class SceneEditorView
    MainController --> ProfileListController
    MainController --> ProfileEditorController
    MainController --> SceneEditorController
    MainController --> Repository
    Controllers --> EventBus
    EventBus --> Navigator
    Navigator --> Views
    ProfileListController --> ProfileListView
    ProfileEditorController --> ProfileEditorView
    SceneEditorController --> SceneEditorView
