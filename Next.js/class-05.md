# Class 05 (21/11/2023)

## Metadata

<meta charset="UTF-8">: This tag is used to specify the character encoding for the document. This is important for ensuring that special characters and non-English text is displayed correctly. THIS IS ALWAYS INCLUDED BY Next.js automatically.

<meta name="viewport" content="width=device-width, initial-scale=1">: This tag is used to control the layout of the page on different devices. It tells the browser to use the device's width as the width of the viewport, and to set the initial zoom level to 1. THIS IS ALWAYS INCLUDED BY NEXT.js automatically.

```

export const metadata = {
  title: "Title of a great page",
  description: "This page is very good",
  robots: "noindex",
  openGraph: {
    title: "title of a great page when shared on facebook",
  },
};

```

description: This tag is used to provide a brief summary of the web page's content. This description is often used by search engines as a snippet when the page appears in search results.

robots: This tag is used to control how search engines index and follow the links on a web page. If a page contains a "noindex" directive, search engines will not include the page in their index. If a page contains a "nofollow" directive, search engines will not follow any links on the page.

This is also where you would include Open Graph tags, to customise your images and metadata on search engines and social network crawlers.

Using meta tags can be beneficial for SEO, better indexing and improving the user experience of your website.

## Dynamic Metadata

```

// Dynamic metadata
export async function generateMetadata({ params }) {
  // you can do any asynchrone js in here, such as load items from a db
  // to get page specific information
  return {
    title: params.pet + " | Pets",
  };
}

```
