```python
from typing import NamedTuple

class ContactInfo(NamedTuple):
    discord: str
    telegram: str

class Attributes:
    def __init__(self):
        self.contact_info = None

        self.life_info = (16, ['Romanian', 'English'])

        self.coding_info = {
            'pro': 'python',
            'intermediate': ('c++','go'),
            'learning': ['js']
        }

        self.specialities = ('web/app reverse engineering', 'automation')
        self.text_editor = ['vscode']

    def get_contact(self) -> ContactInfo:
        return self.contact_info

    def get_life(self):
        return self.life_info

    def get_coding(self):
        return self.coding_info, self.specialities, self.text_editor
```