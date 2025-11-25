# Architecture Overview

```mermaid
classDiagram
    class MainController
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
