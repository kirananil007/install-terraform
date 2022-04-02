# Installing a required version of terraform on Ubuntu 20.04LTS

Terraform is a tool to manage the entire lifecycle of buiding, changing and versioning infrastructure. Terraform works with multiple cloud providers such as Amazon Web Services(AWS), Microsoft Azure, Google Cloud platforms as such or on-prem clouds such as OpenStack, vSphere etc. Hashicorp owns terraform and is open source.

### Install terraform version 1.1.6 on Ubuntu 20.04 LTS
-------------------------------------------------------
1. Set the version required.

            export TF_VERSION=1.1.6

    ![Set Version](/images/tf_version.png "Set TF version")

    <figcaption align="center">Fig 1.a</figcaption>
    
---------------------------------------------------------------------------
2. Download the version of terraform.


        wget https://releases.hashicorp.com/terraform/"${TF_VERSION}"/terraform_"${TF_VERSION}"_linux_amd64.zip

    ![Set Version](/images/download_tf_ver.png)
    <figcaption align="center">Fig 2.a</figcaption>
---------------------------------------------------------------------------

3. Unzip the download file.

        sudo apt install zip -y

    
        sudo unzip terraform_"${TF_VERSION}"_linux_amd64.zip
    ![Set Version](/images/install_zip.png)
    <figcaption align="center">Fig 3.a</figcaption>

    ![Set Version](/images/unzip_tf.png)
    <figcaption align="center">Fig 3.b</figcaption>
    -----------------------------------------------------------------------

4. Move terraform binary to the local/bin.

        sudo mv terraform /usr/local/bin/

    


5. Check terraform version.

        terraform --version
    ![Set Version](/images/get_tf_version.png)
    <figcaption align="center">Fig 4.a</figcaption>

