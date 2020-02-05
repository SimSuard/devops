#BUILD
FROM openjdk:11 AS builder
COPY . .
RUN javac Main.java

#LAUNCH SERVICE
FROM openjdk:11-jre
COPY --from=builder ./Main.class .
CMD java Main
