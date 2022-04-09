
# Install tools required for project
# Run `docker build --no-cache .` to update dependencies
# RUN apt-get update -y
# WORKDIR /application
# COPY requirements.txt . 
# RUN python -m pip install --upgrade pip
# RUN sudo pip install -r requirements.txt
# COPY . .
# EXPOSE 8000
# CMD [ "python3","hello.py"] 

FROM python:latest
WORKDIR /application
COPY . .
RUN apt-get update -y
RUN pip3 install -r requirements.txt
EXPOSE 8000
CMD ["python3","hello.py"]

# List project dependencies with Gopkg.toml and Gopkg.lock
# These layers are only re-built when Gopkg files are updated
# COPY Gopkg.lock Gopkg.toml /go/src/project/
# WORKDIR /go/src/project/
# Install library dependencies
# RUN dep ensure -vendor-only

# Copy the entire project and build it
# This layer is rebuilt when a file changes in the project directory
# COPY . /go/src/project/
# RUN go build -o /bin/project

# This results in a single layer image
# FROM scratch
# COPY --from=build /bin/project /bin/project
# ENTRYPOINT ["/bin/project"]
# CMD ["--help"]
