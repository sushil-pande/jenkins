pipeline
{
    agent any
    stages
    {
        parallel
        {
            stage("A")
            {
                agent aws
                steps
                {
                    echo "========executing A========"
                }   
            }
            stage("C")
            {
                steps
                agent aws
                {
                    echo "====++++executing C++++===="
                }
            }
            stage("D")
            {
                agent aws
                steps
                {
                    echo "====++++executing D++++===="
                }
            }
        }   
    }
}
