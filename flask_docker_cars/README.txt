#------------------------------------------------------------------------------------
# This is a simple web page generated using Docker, Python and Flask
#------------------------------------------------------------------------------------

#------------------------------------------------------------------------------------
# Build an image (Dockerize) and run on Docker container
#------------------------------------------------------------------------------------

cd flask_docker_cars

#------------------------------------------------------------------------------------
# Build image (don't forget the . (point) at the end of the statement)
#------------------------------------------------------------------------------------

docker image build -t flask_cars .

#------------------------------------------------------------------------------------
# Run the container 
#------------------------------------------------------------------------------------

docker run -p 8080:8080 -d flask_cars

#------------------------------------------------------------------------------------
# Open browser
#------------------------------------------------------------------------------------

http://localhost:8080

