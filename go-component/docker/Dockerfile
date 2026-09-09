FROM registry.access.redhat.com/ubi10/go-toolset:1.26-1788946935

COPY . .
RUN go mod download

RUN go build -o ./main

ENV PORT 8081
EXPOSE 8081

CMD [ "./main" ]
