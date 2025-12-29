package com.example.automatetextwriter;

import java.io.IOException;
import java.nio.file.Files;
import java.nio.file.Path;
import java.util.Base64;

public class EncodeDecode1 {

	public static void main(String[] args) throws IOException {
        byte[] fileBytes = Files.readAllBytes(Path.of(""));
        System.err.println(Base64.getEncoder().encodeToString(fileBytes));
        
        byte[] decodedBytes = Base64.getDecoder().decode(base64);
        Files.write(Path.of(""), decodedBytes);

	}
}
