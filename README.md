# Download the Packer file and extract and keep it your c drive
# Configure the Environment variable and add the Packer Path
# Install plugin 
packer plugins install github.com/hashicorp/amazon

# Make Sure to have sufficient permissions for IAM user

# Go to the Path and run the below commands

# packer
packer -v

# To Validate
packer validate --var-file packer-vars.json packer.json

# To Inspect
packer inspect --var-file packer-vars.json packer.json

# To build
packer build --var-file packer-vars.json packer.json
