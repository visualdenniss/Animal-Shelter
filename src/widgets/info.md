# Widgets

Self-sufficient UI blocks that emerged from the composition of lower-level units like entities and features.

This layer provides a way to fill in the slots left in the UI of Entities with other Entities and interactive elements from Features. Therefore, it is common not to have business logic on this layer, instead keeping it in Features. Each slice in this layer contains ready-to-use UI components and sometimes non-business logic such as gestures, keyboard interaction, etc.

Sometimes, however, it is more convenient to have business logic on this layer. Usually it happens when the widget is quite rich in interactivity (e.g., interactive data tables) and the business logic inside them is not used in other places.

**Slice examples:**

For a social network:	
- Post card
- User profile header (with actions)

For a Git frontend (e.g., GitHub):
- List of files in a repository (with actions)
- Comment in a thread
- Repository card