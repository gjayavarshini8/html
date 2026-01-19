node {
    def mvnHome
    stage('Preparation') { // for display purposes
        // Get some code from a GitHub repository
        git branch: 'main',url: 'https://github.com/gjayavarshini8/html.git'
        // Get the Maven tool.
        // ** NOTE: This 'M3' Maven tool must be configured
        // **       in the global configuration.
       
    }
} 
node {

    stage('Stage 1: Clone from GitHub') {
        git branch: 'main',
            url: 'https://github.com/gjayavarshini8/html.git'
    }

    stage('Stage 2: Deploy to Nginx') {
        bat '''
        xcopy /E /Y /I womenclothing\\* C:\\nginx\\nginx-1.28.1\\html
        '''
    }

}
