pipeline{
	agent any
	stages{
		stage('1-clone'){
			steps{
				sh 'pwd'
			}
		}
		stage('2-parallel-jobs'){
			parallel{
				stage('1-saada-subjob1'){
					steps{
						sh 'lscpu'
					}
				}
				stage('2-aubin-subjob2'){
					steps{
						sh 'du -h'
					}
				}
			}
		}
	}
}
