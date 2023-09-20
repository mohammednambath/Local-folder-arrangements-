# Local-folder-arrangements-
files and document arrangement on the local drive
import os

# Define folder names
folders = [
    "Site Survey",
    "AutoCAD",
    "3D Models",
    "Estimation",
    "Authority Approval",
    "Rendering Images",
    "Accounts and Invoice"
]

# Define repository name
repository_name = "Drafting Repository"

# Create main repository folder
os.makedirs(repository_name)

# Create subfolders inside the repository folder
for folder in folders:
    os.makedirs(os.path.join(repository_name, folder))

# Initialize a Git repository
os.system(f'cd "{repository_name}" && git init')

print(f'Folders and repository created successfully in "{repository_name}".')
