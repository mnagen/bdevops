pipeline{





agent any

environment 
{

PATH = "${PATH}:${getTerraformPath()}"
}

stages{

stage('Terraform'){





steps{
sh "terraform init"
}


}



stage('Develop')

{

steps{
echo "Develop"
}

}

stage('Test')

{ 
steps{ 
echo "Testing"

}

}



stage('Deploy') {

steps{
echo "Deploy to production"

}
}

}

}

def getTerraformPath() {
  def tfHome = tool name: 'Terraform', type: 'terraform'
  return tfHome
  }
