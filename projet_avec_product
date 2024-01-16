from flet import app, icons
from flet import MainAxisAlignment
from flet import (
    Card,
    Column,
    Container,
    Divider,
    FilledButton,
    IconButton,
    Markdown,
    Row,
    Text,
    TextField,
)

from product import Product


def main(page):
    page.title = "I Can Has Cheezburger?"
    page.window_width = 400
    page.window_height = 430
    page.add(
        Column(
            alignment=MainAxisAlignment.CENTER,
            controls=[
                Product("🍔", 5.95),
                Product("🍟", 3.60),
                Product("🥗", 8.30),
                Product("🥤", 2.60),
                Divider(),
                Row(
                    [
                        Card(
                            Container(
                                Markdown(
                                    "**TOTAL:** 0.00 €"
                                ),
                                padding=10,
                            )
                        ),
                        FilledButton(
                            text="Buy", icon=icons.PAYMENT
                        ),
                    ],
                    alignment=MainAxisAlignment.SPACE_BETWEEN,
                ),
            ],
        )
    )


app(target=main)