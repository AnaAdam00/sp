# sp
package com.company;
import java.util.Collections;
import java.util.List;

public class Book {
    private String title;
    private List<String> paragraph;
    private List<String> images;
    private  List<String>tables;
    public Book(String title){
        this.title= title;
    }



    public void createNewParagraph(String paragraph){
        this.paragraph.add(paragraph);
    }
    public void createNewImages(String images){
        this.images.add(images);
    }
    public void createNewTable(String tables){
        this.tables.add(tables);
    }
    public void print(){
        System.out.println("Titlul: %s"+title);
        System.out.println("Paragrafele:");
        for(String i : this.paragraph)
            System.out.println(i);

        System.out.println("Imaginile:");
        for(String i : this.images)
            System.out.println(i);

        System.out.println("Tabele:");
        for(String i : this.tables)
            System.out.println(i);
    }
}

