pipeline{
    agent {
        docker { image 'mdsol/python2'}
    }
    stages{
        stage('Build'){
            steps{
                sh 'python -m py_compile sources/add2vals.py sources/calc.py'
                stash(name: 'compiled-results', includes: 'sources/*.py*')
            }
        }
    }
}