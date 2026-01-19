node {

    stage('Preparation') {
        git branch: 'main',
            url: 'https://github.com/Anubhav2004/Devops_project.git'
    }

    stage('Copy to Test Unit 45') {
        bat '''
        if not exist C:\\jenkins\\test-units\\45 mkdir C:\\jenkins\\test-units\\45
        xcopy /E /I /Y "%WORKSPACE%\\*" "C:\\jenkins\\test-units\\45\\"
        '''
    }
}
